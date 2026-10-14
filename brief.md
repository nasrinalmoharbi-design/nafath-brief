Version: NAFATH-V1
Track: Cybersecurity

## Overview

NAFATH-V1 is a proposed national login service that helps citizens access government services securely. It connects six IT areas: Software, AI, Mobile, Networking, Cybersecurity, and Data. Each area has an important role. Software manages login and access, AI helps identify unusual activity, and Mobile provides access through phones. Networking protects communication, Cybersecurity helps defend against attacks, and Data practices protect personal information. All six areas must work together to make the service secure, reliable, and easy to use.

## Software


OAuth 2.0 and OpenID Connect have different purposes. OAuth 2.0 allows an application to access protected resources with permission. OpenID Connect (OIDC) adds an identity layer to OAuth 2.0 and is designed for user login. In the national login service, OIDC helps confirm the citizen’s identity, while OAuth 2.0 controls access to protected services. Both work together to support secure access to government services.

Resource: OpenID Connect Core 1.0 - https://openid.net/specs/openid-connect-core-1_0.html

## AI
AI can help detect suspicious logins by identifying unusual patterns, such as logins from unexpected locations or devices. Before using the model, the authority should assess privacy, bias, security, accuracy, and the risk of false alerts. The NIST AI Risk Management Framework recommends managing AI risks through the functions Govern, Map, Measure, and Manage. Human review, testing, monitoring, and clear accountability should be in place before launch.

Resource: NIST AI Risk Management Framework - https://www.nist.gov/itl/ai-risk-management-framework

## Mobile
Android uses a runtime permission model to control access to sensitive features and data on a device. An app must request permission when it needs a protected resource, such as the camera or location, and the user must approve the request when required. The login app should request only necessary permissions, explain why they are needed, and respect the user’s choice. This reduces unnecessary access to personal information.

Resource: Android Developers - Request app permissions - https://developer.android.com/training/permissions/requesting

## Networking
DNS over HTTPS (DoH) sends DNS queries through encrypted HTTPS connections. It helps protect citizens’ domain lookups from being easily read or modified by someone monitoring the network. However, DoH does not hide all internet activity, encrypt every connection, or guarantee that a website is safe. The login service should use secure HTTPS connections and other security controls as well.

Resource: RFC 8484 - DNS Queries over HTTPS (DoH) - https://www.rfc-editor.org/rfc/rfc8484


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
