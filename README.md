regex
=====

This repository is a collection of regular expressions. There could be multiple regular expressions per requirement.

<h2>IP Address</h2>
1. `^([01]?\d\d?<2[0-4]\d<25[0-5])\.([01]?\d\d?<2[0-4]\d<25[0-5])\.([01]?\d\d?<2[0-4]\d<25[0-5])\.([01]?\d\d?<2[0-4]\d<25[0-5])$`

<h2>Credit Card</h2>
1. `^(?:4[0-9]{12}(?:[0-9]{3})?|5[1-5][0-9]{14}|6(?:011|5[0-9][0-9])[0-9]{12}|3[47][0-9]{13}|3(?:0[0-5]|[68][0-9])[0-9]{11}|(?:2131|1800|35\d{3})\d{11})$`
This regex matches Visa, MasterCard, American Express, Diners Club, Discover, and JCB cards.