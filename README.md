# Unauthenticated Scan

![image](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/02fa4e0d-af3c-45ea-827e-058555314f36)

## Intro

I will use OpenVAS to scan the vulnerable virtual machine:
- It will be an unauthenticated scan.
  * That means the vulnerability management platform wont login the computer and look indepth at it.
  * It's like a superficial scan and I will use the results and compare it to the authenticated scan.

- I will log into OpenVAS.
- I will add the Windows virutal machine private IP address in OpenVAS
  * To get tge private IP address, I went back to the Azure portal.
  * Then I went to the Windows virutal machine and copied it.
![VL 20](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/0e23e2d7-235b-4e40-ba8c-b94c53e152ce)

- Back in OpenVAS, I will click Assets, then click Hosts, then click New Host

![VL 19](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/bdeb95b2-9ed3-4539-9d3d-d8ff99eaf5cd)

- I pasted the private IP address in the New Host.
- Gave it the name "Win10-Vulnerable"
- And click Save

![VL 21](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/f98b991d-3609-4d8d-9758-8cc6aa70dee8)

- Now I will create a New Target from Host and call it "Azure Vulnerable VMs"
![VL 22](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/03fda584-3b13-4cd0-8993-8c728dd3f9cf)
![VL 23](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/a26651da-92ee-49ef-8355-0769cb695cc4)


- Now I will create a New Task to conduct the scan.
- I went to scans in OpenVAS and click task.
![VL 24](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/17343a40-811e-46d3-90ee-4b24507556a9)
![VL 25](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/ec40ae79-5f22-470e-b064-3e6e78d42984)


- I will call the scan: "Scan-Azure Vulnerable VMs"
- The scan target will be: Azure Vulnerable VMs
- And click save

![VL 26](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/ea813d28-3580-459d-bb53-30cb6e259f45)



- The task has been created.
- Click the start button to begin scanning.
![VL 27](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/7ceb6905-79ee-4e0b-8e70-7e00606334f7)


- The scan will take awhile to complete.
  * Wait for it to be done.
![VL 28](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/6fdca55a-2f7f-4449-86f0-7ac7863b07ff)

- Clicked on "Report" to see the results
  * Remember, I didn't do an authenticated scan so less vulnerabilites showed up.
  * The insecure softwares didn't show up.
![VL 29](https://github.com/Ashrafs-Tech/Configure-OpenVAS/assets/166546026/2d8fa737-8793-47a7-a4ef-e52e795cb81f)


## Step 4 is done.

An unauthenticated scan has been completed.

