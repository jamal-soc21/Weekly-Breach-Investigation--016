Weekly Breach Investigation
Breach: Adform — Malicious JavaScript Supply‑Chain Attack
Analyst: Jamal Mahmoad
Date: 2026‑08-01

Summary
"Attackers modified Adform’s trackpoint-async.js script into a browser‑side wallet address rewriter."

"Victims copying or entering Bitcoin, Ethereum, or Tron addresses risked silent replacement."

"Incident detected and removed by Adform on July 27, but cached copies may persist."

"No persistence or software installation; malicious code only active while page remained open."

Attack Flow
"Shared Adform script compromised → downstream websites exposed."

"Clipboard monitored every 4 seconds; addresses replaced."

"Text nodes and input fields rewritten in real time."

"Obfuscated replacement strings via XOR key."

"HTTP beacon attempted to send hostname/path to external server (84.32.102[.]230:7744)."

MITRE ATT&CK
"Initial Access: Supply‑Chain Compromise (T1195)"

"Execution: Malicious JavaScript in Browser (T1059.007)"

"Collection: Clipboard & Input Hijacking (T1119)"

"Exfiltration: HTTP Beacon to External Server (T1041)"

Mitigation
"Clear browser cache to remove cached malicious script."

"Verify wallet addresses before sending funds."

"Monitor shared third‑party resources for tampering."

"Implement integrity checks (Subresource Integrity, CSP)."

Analyst Notes
"Incident highlights risks of shared advertising/tracking scripts as supply‑chain vectors."

"Scope remains unclear: number of sites, visitors, and diverted funds not published."

"Timeline discrepancy between Adform’s July 27 statement and researcher observations."

"Demonstrates how one compromised resource can cascade across unrelated websites."
