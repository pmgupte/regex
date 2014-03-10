<h1>regex</h1>
This repository is a collection of regular expressions. There could be multiple regular expressions per requirement.

<h2>Table of Contents</h2>
1. [IP Address](#ip-address)
2. [Credit Card](#credit-card)
3. [Hex Color Code](#hex-color-code)
4. [UUID/GUID](#uuidguid)
5. [Email Address](#email-address)
6. [Base64 Encode](#base64-encode)
7. [Date and Time](#date-and-time)

<h2>IP Address</h2>
1. `^([01]?\d\d?<2[0-4]\d<25[0-5])\.([01]?\d\d?<2[0-4]\d<25[0-5])\.([01]?\d\d?<2[0-4]\d<25[0-5])\.([01]?\d\d?<2[0-4]\d<25[0-5])$`

<h2>Credit Card</h2>
1. `^(?:4[0-9]{12}(?:[0-9]{3})?|5[1-5][0-9]{14}|6(?:011|5[0-9][0-9])[0-9]{12}|3[47][0-9]{13}|3(?:0[0-5]|[68][0-9])[0-9]{11}|(?:2131|1800|35\d{3})\d{11})$`
This regex matches Visa, MasterCard, American Express, Diners Club, Discover, and JCB cards.

<h2>Hex Color Code</h2>
1. `^#(?:[0-9a-fA-F]{3}){1,2}$`
2. `^#([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$`

<h2>UUID/GUID</h2>
1. `^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$`
2. `/^[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}$/i`
This one is implied regex, and seems that this one is better than regex no. 1.

<h2>Email Address</h2>
1. `^[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,4}$`

<h2>Base 64 Encode</h2>
1. `[^-A-Za-z0-9+/=]|=[^=]|={3,}$`
2. `^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==|[A-Za-z0-9+/]{3}=)?$`

<h2>Date and Time</h2>
1. `^(0?[1-9]|[12][0-9]|3[01])[\/\-\.](0?[1-9]|1[012])[\/\-\.](\d{4})\s([0-1][0-9]|[2][0-3])\-([0-5][0-9])\-([0-5][0-9])$`