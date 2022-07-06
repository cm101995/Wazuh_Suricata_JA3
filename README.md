# Wazuh_Suricata_JA3

This code helps in comparing the JA3 hashes against the malicious ones from abuse.ch website. 

Prerequisites:
1)Suricata logs are being sent to Wazuh
2)Have malicious JA3 hashes locally within Wazuh directory

1) Download the malicious hashes locally (https://sslbl.abuse.ch/blacklist/ja3_fingerprints.csv)
2) Create a custom active response rule in Wazuh.


Reference:
1)https://documentation.wazuh.com/current/user-manual/capabilities/active-response/custom-active-response.html
2)https://abuse.ch/
