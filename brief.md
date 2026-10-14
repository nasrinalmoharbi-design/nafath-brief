Version: NAFATH-V1
Track: Cybersecurity

## Overview

NAFATH-V1 is a proposed national login service that helps citizens access government services securely. It connects six IT areas: Software, AI, Mobile, Networking, Cybersecurity, and Data. Each area has an important role. Software manages login and access, AI helps identify unusual activity, and Mobile provides access through phones. Networking protects communication, Cybersecurity helps defend against attacks, and Data practices protect personal information. All six areas must work together to make the service secure, reliable, and easy to use.

## Software




Software helps NAFATH-V1 verify users and give them access to the correct services. OAuth 2.0 allows applications to access protected resources with permission. OpenID Connect (OIDC) helps confirm a user’s identity during login. Using these standards correctly can make the login process more secure and help protect government services from unauthorized access.

Resource: OpenID Foundation — OpenID Connect Core 1.0
https://openid.net/specs/openid-connect-core-1_0.html


## AI


AI can help NAFATH-V1 detect unusual login activity, such as repeated failed login attempts or logins from unexpected locations. However, AI can make mistakes and may identify normal activity as suspicious. The system should be tested regularly, protect users’ personal information, and allow security staff to review alerts. This helps make AI more reliable and reduces the risk of incorrect decisions.

Resource: NIST — AI Risk Management Framework
https://www.nist.gov/itl/ai-risk-management-framework

## Mobile

The NAFATH-V1 mobile app should protect users’ information and privacy. Android apps must request permission before accessing protected features, such as the camera or location, when required. The app should ask only for permissions it needs and explain why they are necessary. This helps users understand how their information is used and reduces unnecessary access to personal data.

Resource: Android Developers — Request App Permissions
https://developer.android.com/training/permissions/requesting


## Networking

Networking allows the NAFATH-V1 mobile app and servers to communicate securely. HTTPS helps protect information while it travels between the app and the server. DNS over HTTPS (DoH) encrypts DNS queries, making them harder for others on the network to read or change. However, DoH does not protect all internet activity or guarantee that a website is safe. NAFATH-V1 should use secure communication protocols and proper network security controls to protect users’ information.

Resources:

* IETF RFC 8484 — DNS Queries over HTTPS (DoH): https://www.rfc-editor.org/rfc/rfc8484
* IETF RFC 8446 — TLS 1.3: https://www.rfc-editor.org/rfc/rfc8446
* 3GPP — Mobile Network Standards: https://www.3gpp.org/

## Cybersecurity


Cybersecurity protects NAFATH-V1 from attacks and unauthorized access. Attackers may use phishing to trick users into sharing their passwords or verification codes. The service should use strong authentication, control access to sensitive information, and monitor suspicious activity. Passkeys and security keys based on FIDO2 or WebAuthn can help prevent phishing when implemented correctly. These measures help protect citizens’ accounts and personal information.

Resources:

* NIST — Digital Identity Guidelines: https://pages.nist.gov/800-63-4/sp800-63b.html
* W3C — Web Authentication (WebAuthn): https://www.w3.org/TR/webauthn-3/

## Data


NAFATH-V1 must protect citizens’ personal information. The service should collect only the data it needs and explain why the data is collected. Access to personal information should be limited to authorized people, and stored data should be protected from unauthorized access. The service must also follow Oman’s Personal Data Protection Law and applicable regulations. These practices help protect privacy and build citizens’ trust in the service.

Resource: Oman Personal Data Protection Law — Royal Decree 6/2022
https://qanoon.om/p/2022/rd20220006/


## Misconception in My Track
A common misconception is that using multi-factor authentication (MFA) automatically makes every login phishing-resistant. MFA adds extra verification, but attackers may still steal passwords and one-time codes through fake websites. Phishing-resistant methods, such as correctly implemented FIDO2 security keys or passkeys, bind authentication to the legitimate website and make credential theft harder. Therefore, the national login service should not treat all MFA methods as equally resistant to phishing.

## Open Question
How can the authority make phishing-resistant authentication easy for all citizens to use, including people with older devices or limited technical skills?
