# Purge-LFM
Deletes entire history from Last.FM

[[insert video link here]]

straight up stolen from https://gist.github.com/teknikqa/f14fa07cf28228cb2dfe49a0caab8e70
dfbadawi's code with minor changes
used this for my alternate account. would NOT recommend using on a main account as it will delete until you make it stop. Copy into console if you just want to delete one page.

replace the URL with your library page's URL
The second time I ran this method, I kept getting an error screen so the URL will get the process back on track if that happens.

Use this or a similar extension: https://chrome.google.com/webstore/detail/run-javascript/lmilalhkkdhfieeienjbiicclobibjao/related

and copy the following code into it

```
jQuery('button.dropdown-menu-clickable-item[data-ajax-form-sets-state=deleted]').each(function(_, b) {
  b.click();
});
window.location.replace("https://www.last.fm/user/***YOUR_USERNAME_HERE***/library")
```
