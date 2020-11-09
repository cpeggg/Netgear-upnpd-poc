# Netgear-upnpd-poc

Netgear upnpd request process stack overflow.

Any user can get remote code execution through LAN, this vulnerability currently affects latest R、RAX、XR series, including R6400v2(V1.0.4.102_10.0.75), R6400(V1.0.1.62_1.0.41), R7000P(V1.3.2.126_10.1.66), XR300(V1.0.3.50_10.3.36), R8000(V1.0.4.62), R8300(V1.0.2.136), R8500(V1.0.2.136), R7300DST(V1.0.0.74), R7850(V1.0.5.64), R7900(V1.0.4.30), R8000(V1.0.4.62), R8300(V1.0.2.136), R8500(V1.0.2.136), RAX20(V1.0.2.64), RAX80(V1.0.3.102), R6250(V1.0.4.44), we believe there are much more models suffered from this vuln.

## Vulnerability description

This vulnerability happen when upnpd receive and process specific message and copy the user data the stack buffer, attackers can exploit this to get remote code execution.

## Poc

refer to this video: [pov.mkv](https://github.com/cpeggg/Netgear-upnpd-poc/)

## Timeline

2020.11.7 report to tianfucup;

2020.11.9 report to cve and netgear
