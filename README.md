# Direct Send Abuse - Header Analyzer
Paste message headers, click **Analyze**, and see whether the email matches a typical Direct Send abuse profile.

https://jasonsford.github.io/directsendanalyzer

## What is Direct Send Abuse?
Attackers abuse the Direct Send feature in Microsoft 365, which is intended to allow legacy applications and devices like multi-function copiers to send email. These messages:

* Spoof an internal user in both the To and From address
* Have a Microsoft EOP SCL score of 0 or 1
* Fail SPF, DKIM, and DMARC

The tool applies those indicators, drawn from research on Direct Send abuse attacks:  
<https://www.proofpoint.com/us/blog/email-and-cloud-threats/attackers-abuse-m365-for-internal-phishing>

## How to use this tool
1. Open the **Header Analyzer** link.  
2. Copy the full message headers from Outlook (Ctrl+F1 → *Message Options*).  
3. Paste them into the text box.
4. Click **Analyze**.  
5. Review the color‑coded table and verdict.

**<span style="color:#14892c;">Green</span>** = the message headers match the criteria for a Direct Send abuse attack.

**<span style="color:#d73a49;">Red</span>** = the message headers do **not** match the criteria for a Direct Send abuse attack.

## Contributing
Pull requests are welcome. For major changes, please open an issue to discuss what you would like to change.

Code can be customized for other hosted email security platforms by swapping out *.pphosted.com for the domain belonging to the appropriate provider.

## Authors
[Jason Ford](http://jasonsford.com)

## License
[GPLv3](https://choosealicense.com/licenses/gpl-3.0/)
