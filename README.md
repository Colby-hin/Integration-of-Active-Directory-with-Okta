# Integrating Active Directory with Okta 

---
Started the process to integrate my on-premises Active Directory with Okta from the Directory Integrations section in the Okta Admin Console. 

<img width="1530" height="850" alt="Screenshot 2025-10-11 184053" src="https://github.com/user-attachments/assets/b105c882-0429-4c02-877e-3be8d187d770" />

---
Okta requires the AD Agent to be installed on a Windows Server 2016 or later that’s joined to the same domain. The agent connects Okta to AD securely for provisioning and authentication.
<img width="815" height="681" alt="Screenshot 2025-10-11 184700" src="https://github.com/user-attachments/assets/c6f12d82-7b8d-4713-9133-152b50800cca" />



---

Began setup by downloading the Okta Active Directory Agent, which handles communication between Okta and the domain controller.

<img width="1541" height="800" alt="Screenshot 2025-10-11 185715" src="https://github.com/user-attachments/assets/5f1b5664-77ed-4ba4-876d-013770dee310" />

---
Installed the agent on the server and configured it to run using a domain service account that has directory access.
<img width="1550" height="800" alt="Screenshot 2025-10-11 190826" src="https://github.com/user-attachments/assets/2cf28680-85fd-4f9a-8d39-d0fe04aba7d7" />

---
Registered the Okta AD Agent with the Okta tenant by authorizing the connection to securely link my AD environment to Okta.
<img width="1540" height="790" alt="Screenshot 2025-10-11 190942" src="https://github.com/user-attachments/assets/757ac156-b4e2-4fc3-ae94-53e58334ef6d" />

---

<img width="1557" height="804" alt="Screenshot 2025-10-11 191029" src="https://github.com/user-attachments/assets/1c2a6e63-245c-46d8-b428-7e0327dc5325" />

---

<img width="1534" height="795" alt="Screenshot 2025-10-11 191047" src="https://github.com/user-attachments/assets/3006bf07-7c91-414e-81d8-2079cbb7cb26" />

---
Selected specific OUs (HR and IT) to sync users and groups from Active Directory to Okta.
<img width="1549" height="839" alt="Screenshot 2025-10-11 191145" src="https://github.com/user-attachments/assets/f95130b9-c060-499c-a893-fc01a15e6e9c" />

---
Once setup was complete, Okta confirmed that the Active Directory domain was successfully integrated, allowing synchronization and delegated authentication.
<img width="1709" height="940" alt="Screenshot 2025-10-11 191715" src="https://github.com/user-attachments/assets/99b6e17e-f5bd-4c27-869e-311d1ecf795f" />


---


<img width="1910" height="1011" alt="Screenshot 2025-10-11 192526" src="https://github.com/user-attachments/assets/966f6e60-949f-403a-ae53-8dbc5995f80e" />

---
Configured user import rules and selected how Okta generates usernames — for example, using SAM Account Name or UPN.
<img width="795" height="628" alt="Screenshot 2025-10-11 193331" src="https://github.com/user-attachments/assets/10628173-a120-4ceb-b7aa-8f933ed0d87d" />

---
Enabled additional settings:

JIT Provisioning: Allows automatic user account creation when they first log in.

<img width="804" height="606" alt="Screenshot 2025-10-11 193454" src="https://github.com/user-attachments/assets/cdf18610-9e28-4644-8201-81b90a6ff6d7" />

---
Auto-activate new users: New user accounts are automatically activated upon creation, so they are ready to be used immediately without a manual administrator action.
<img width="907" height="649" alt="Screenshot 2025-10-11 193758" src="https://github.com/user-attachments/assets/85861d44-254c-4df3-ad96-d2a0c8f4ec63" />

---

<img width="1919" height="1045" alt="Screenshot 2025-10-11 193959" src="https://github.com/user-attachments/assets/aa3f0117-f5c4-42e3-ae8a-4d692162e262" />

---

<img width="1912" height="977" alt="Screenshot 2025-10-11 194054" src="https://github.com/user-attachments/assets/28c3a839-252e-458f-b7cd-e9368bb060d2" />

---

Manual import lets you pick which specific users to bring into Okta, while auto import would add all detected users automatically.
<img width="1145" height="707" alt="Screenshot 2025-10-11 194330" src="https://github.com/user-attachments/assets/e645b0e7-4add-4bdc-88ab-0be611ae25dc" />

---

I went to the "People" tab and saw the selected users were added in.
<img width="1903" height="981" alt="Screenshot 2025-10-11 194519" src="https://github.com/user-attachments/assets/e76f9430-35dc-4d35-840e-621bf1adbf3c" />


With the users that were not activated yet i activated here.
<img width="1914" height="972" alt="Screenshot 2025-10-11 194729" src="https://github.com/user-attachments/assets/374f792f-cc41-4f34-82af-81baea8f8289" />



