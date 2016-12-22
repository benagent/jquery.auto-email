# jquery.auto-email
### An autocomplete JQuery plugin for email fields

This plugin autocompletes email addresses when supplied with an email domain.  Instead of the regular jQuery autocomplete's dropdown menu of autocomplete suggestions, this types ahead while keeping the auto-filled text highlighted as to not obstruct the user.

### Demo

https://demos.hisune.com/jquery-auto-email

### To use this plugin, download the file and on pageload, call:

```javascript
$('#your-field').autoEmail(["gmail.com", "foo.org", "foo.com", "foobar.com"], "gmail.com", false);
```

The method accepts three parameters, `domains` and `defaultDomain` and `multi-enabled`.

* `domains` is an array of domains to autocomplete with, autocompleting on the first match in the array.  Typing `joe@f` in the above example will first autocomplete to `joe@foo.org`.  After the user types `joe@foob`, the field will autocomplete to `joe@foobar.com`.
* `defaultDomain` is a string of your precedence domain to match.
* `multi-enabled` is a boolean flag that enables the user to enter multiple emails in the field, separated by a `,` or `;`

