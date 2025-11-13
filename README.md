# Elevate-Labs-internship-work

The target hosts had the following open ports:

Common Open Ports Identified

135/tcp – MSRPC

445/tcp – SMB (microsoft-ds)

1001/tcp – Webpush / Custom service

9080/tcp – gRPC / Web service

53/tcp – DNS

⚠️ Security Risks Associated With These Ports Port 135 – MSRPC

Frequently targeted in Windows-based attacks

Previously exploited by worms like Blaster

May leak system information Risk Level: High

Port 445 – SMB (microsoft-ds)

Known for major exploits such as EternalBlue

Can allow remote code execution

Enables unauthorized file access and lateral movement Risk Level: Critical

Port 1001 – Custom Service

Non-standard port → high chance of weak security

Could expose internal APIs

May expose debugging interfaces Risk Level: Medium

Port 9080 – Web/gRPC Service

Often used for admin panels or backend services

If left unprotected, could allow unauthorized access Risk Level: Medium to High

Port 53 – DNS

May be vulnerable to DNS amplification attacks

Misconfigurations could leak internal hostname information Risk Level: Medium

The scan identified several services that could pose security risks if exposed to a public or untrusted network. High-risk services such as SMB (445) and MSRPC (135) should be secured, restricted, or disabled if not needed.

This completes the task of scanning the network, analyzing the open ports, and identifying the associated risks.
