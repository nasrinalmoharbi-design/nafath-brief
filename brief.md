Version: NAFATH-V1
Track: Cybersecurity

## Overview
A secure national login service must connect six IT fields rather than treat them as separate tasks. Software standards help the website and mobile app confirm a user’s identity and grant access to the appropriate services. AI can flag unusual login patterns, but its alerts need testing, human review, and safeguards against incorrect decisions. The mobile app should request Android permissions only when needed and explain their purpose. Networking protections such as DNS over HTTPS can reduce exposure of domain lookups, although they do not encrypt all activity or prove that a website is trustworthy. Cybersecurity controls must protect accounts against phishing and account takeover. Data practices must follow Oman’s personal data law and use appropriate safeguards. Together, these choices can make the service secure, reliable, and easier for citizens to use.

## Software
Software

OAuth 2.0 and OpenID Connect have different purposes. OAuth 2.0 allows an application to access protected resources with permission. OpenID Connect (OIDC) adds an identity layer to OAuth 2.0 and is designed for user login. In the national login service, OIDC helps confirm the citizen’s identity, while OAuth 2.0 controls access to protected services. Both work together to support secure access to government services.

Resource: OpenID Connect Core 1.0 - https://openid.net/specs/openid-connect-core-1_0.html

## AI
AI can help detect suspicious logins by identifying unusual patterns, such as logins from unexpected locations or devices. Before using the model, the authority should assess privacy, bias, security, accuracy, and the risk of false alerts. The NIST AI Risk Management Framework recommends managing AI risks through the functions Govern, Map, Measure, and Manage. Human review, testing, monitoring, and clear accountability should be in place before launch.

Resource: NIST AI Risk Management Framework - https://www.nist.gov/itl/ai-risk-management-framework

## Mobile
Android uses a runtime permission model to control access to sensitive features and data on a device. An app must request permission when it needs a protected resource, such as the camera or location, and the user must approve the request when required. The login app should request only necessary permissions, explain why they are needed, and respect the user’s choice. This reduces unnecessary access to personal information.

Resource: Android Developers - Request app permissions - https://developer.android.com/training/permissions/requesting

## Networking


## Cybersecurity


## Data

## Misconception in My Track

## Open Question
