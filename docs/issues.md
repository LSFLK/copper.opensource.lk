# Common issues for email solutions

## Threats
<p align="justify">
Eventhough the Email is one of the main communication model in the world now it has some information security issues too. Hear we just trying to high light them to grab your attention over those issue while you are operating any email solution.
</p>


## Spam
<p align="justify">
Irrelevant or unsolicited(unrequested) messages sent over the Internet, typically to a large number of users, for the purposes of advertising, phishing, spreading malware, etc.
</p>

## Spoofing
<p align="justify">
Email spoofing is one of the best known spoofs. Since core SMTP fails to offer authentication, it is simple to forge and impersonate emails. Spoofed emails may request personal information and may appear to be from a known sender. Such emails request the recipient to reply with an account number for verification. The email spoofer then uses this account number for identity theft purposes, such as accessing the victim’s bank account, changing contact details and so on.” [https://www.techopedia.com/definition/5398/spoofing]
</p>

## Phishing
<p align="justify">
The fraudulent practice of sending emails purporting(appear to be or do something, especially falsely.) to be from reputable companies in order to induce individuals to reveal personal information, such as passwords and credit card numbers.

Here are a few steps a company can take to protect itself against phishing according to 
web site "https://digitalguardian.com/blog/phishing-attack-prevention-how-identify-avoid-phishing-scams".

    Educate your employees and conduct training sessions with mock phishing scenarios.
    Deploy a SPAM filter that detects viruses, blank senders, etc.
    Keep all systems current with the latest security patches and updates.
    Install an antivirus solution, schedule signature updates, and monitor the antivirus status on all equipment.
    Develop a security policy that includes but isn't limited to password expiration and complexity.
    Deploy a web filter to block malicious websites.
    Encrypt all sensitive company information.
    Convert HTML email into text only email messages or disable HTML email messages.
    Require encryption for employees that are telecommuting.

In copper RSPAMD spam filter is deployed. But most of other steps to be taken by the clients who are copper mail solution is to be used.

</p>


## Malware
<p align="justify">
software that is specifically designed to disrupt, damage, or gain unauthorized access to a computer system.
To controll malware attack, clamav is installed in emailserver image and will be updated for each 50 minutes.
</p>


## Solutions

## Mail Filtering
<p align="justify">
Mail Filtering is widely used to avoide spams and many tools are used to achive this target. DKIM and SPF are two of such mail filtering tools. Sender Policy Framework (SPF) is an email validation protocol designed to detect and block email spoofing by providing a mechanism to allow receiving mail exchangers to verify that incoming mail from a domain comes from an IP Address authorized by that domain’s administrators.
Copper email solution has used both of above technologies to filter mails.
"DomainKeys Identified Mail (DKIM) is an email authentication method designed to detect forged sender addresses in emails (email spoofing), a technique often used in phishing and email spam.
DKIM allows the receiver to check that an email claimed to have come from a specific domain was indeed authorized by the owner of that domain. It achieves this by affixing a digital signature, linked to a domain name, to each outgoing email message. The recipient system can verify this by looking up the sender's public key published in the DNS. A valid signature also guarantees that some parts of the email (possibly including attachments) have not been modified since the signature was affixed. Usually, DKIM signatures are not visible to end-users, and are affixed or verified by the infrastructure rather than the message's authors and recipients" (https://en.wikipedia.org/wiki/DomainKeys_Identified_Mail).


</p>


## Transport encryption
<p align="justify">
Transport encryption means that the email(s) will be encrypted when they are send (transferred) from one server to another. The emails are send through an encrypted tunnel when using this method. The emails are encrypted when the depart from one server and decrypted when the arrive on the other server. All emails on the server are not encrypted when they are stored on the server. Sending encrypted emails over the internet you would use for example the POP3S email transfer protocol with the Transport Layer Security (TLS)network protocol (which is the new name for the Secure Sockets Layer (SSL) protocol used for quite some years now).

In copper email solution uses mycrypt to encript mail dir. 
Communication between ldap server and smtp server and imap server are tls enabled.


</p>