Version: NAFATH-V1
Track: Cybersecurity

## Overview

NAFATH-V1 is a proposed national login service that helps citizens access government services securely. It connects six IT areas: Software, AI, Mobile, Networking, Cybersecurity, and Data. Each area has an important role. Software manages login and access, AI helps identify unusual activity, and Mobile provides access through phones. Networking protects communication, Cybersecurity helps defend against attacks, and Data practices protect personal information. All six areas must work together to make the service secure, reliable, and easy to use.

## Software


Software

Software helps NAFATH-V1 verify users and give them access to the correct services. OAuth 2.0 allows applications to access protected resources with permission. OpenID Connect (OIDC) helps confirm a user’s identity during login. Using these standards correctly can make the login process more secure and help protect government services from unauthorized access.

Resource: OpenID Foundation — OpenID Connect Core 1.0
https://openid.net/specs/openid-connect-core-1_0.html


## AI


AI can help NAFATH-V1 detect unusual login activity, such as repeated failed login attempts or logins from unexpected locations. However, AI can make mistakes and may identify normal activity as suspicious. The system should be tested regularly, protect users’ personal information, and allow security staff to review alerts. This helps make AI more reliable and reduces the risk of incorrect decisions.

Resource: NIST — AI Risk Management Framework
https://www.nist.gov/itl/ai-risk-management-framework


## Cybersecurity
Phishing-resistant authentication helps prevent attackers from stealing login credentials through fake websites. Passkeys using FIDO2 or WebAuthn can provide phishing-resistant authentication when correctly implemented. SMS codes and one-time passwords entered into a fake website are not phishing-resistant because attackers may steal and reuse them. The national login service should prefer phishing-resistant methods to protect citizens’ accounts.

Resource: NIST SP 800-63B - Digital Identity Guidelines - https://pages.nist.gov/800-63-4/sp800-63b.html

## Data
Oman’s Personal Data Protection Law requires organizations to handle personal data according to legal obligations. The authority should identify a lawful basis for processing, explain the purpose of collection, protect stored data, and respect individuals’ rights. It should also follow applicable rules for consent, data sharing, retention, and cross-border transfers. Legal and privacy teams should verify the requirements before the service launches.

Resource: Oman Personal Data Protection Law, Royal Decree 6/2022 - https://qanoon.om/p/2022/rd20220006/

## Misconception in My Track
A common misconception is that using multi-factor authentication (MFA) automatically makes every login phishing-resistant. MFA adds extra verification, but attackers may still steal passwords and one-time codes through fake websites. Phishing-resistant methods, such as correctly implemented FIDO2 security keys or passkeys, bind authentication to the legitimate website and make credential theft harder. Therefore, the national login service should not treat all MFA methods as equally resistant to phishing.

## Open Question
How can the authority make phishing-resistant authentication easy for all citizens to use, including people with older devices or limited technical skills?
