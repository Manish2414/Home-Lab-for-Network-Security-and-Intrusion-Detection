# Home Lab for Network Security and Intrusion Detection

## Overview

This project demonstrates the construction of a dynamic virtualized network using VirtualBox, featuring OPNsense as the primary firewall solution, Kali Linux for penetration testing, and Windows as the target system. The objective is to showcase proficiency in virtualization technologies while enhancing network security through proactive measures such as intrusion detection and vulnerability assessments.

![Kali Linux and OPNsense](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700423038/screenshots2/main_pic_zsaybu.png)

## Technologies Used

- **Virtualization:** VirtualBox
  
  Download VirtualBox: https://www.virtualbox.org/wiki/Downloads
- **Firewall Solution:** OPNsense
  
  Download OPNsense ISO: https://opnsense.org/download/
- **Penetration Testing:** Kali Linux
  
  Download Kali Linux ISO: https://www.kali.org/get-kali/#kali-platforms
- **Target System:** Windows
  
  Download Windows ISO: https://www.microsoft.com/en-us/software-download/windows10ISO

  ![All VMs on virtual box](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700423039/screenshots2/all_vms_for_homelab_ym3uex.png)

## Features

1. **OPNsense Configuration:**
   - Deployed and configured OPNsense as the primary firewall solution.
   - Implemented [custom Nmap rules](customnmap.rules) to intelligently detect and alert scanning activities.

  ![OPNsense](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700423039/screenshots2/OPNsense_homescreen_waiyuc.png)

  ![Nmap rule](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700423039/screenshots2/nmap_rule_pluhid.png)

2. **Intrusion Detection:**
   - Utilized Suricata for intrusion detection.
   - Configured firewall rules to enhance security.
   - Executed tests to detect and alert to potential threats.

  ![Nmap test](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700423039/screenshots2/nmap_test_znthsw.png)

  ![Alerts](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700423039/screenshots2/IDS_Alerts_hva3wo.png)

3. **Vulnerability Assessments:**
   - Conducted vulnerability assessments on the network.
   - Implemented measures to fortify the network against potential threats.

4. **Monitoring and Log Analysis:**
   - Enhanced cybersecurity measures through proactive detection.
   - Monitored network activities and performed log analysis.

   ![Log files](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700423837/screenshots2/log_files_jqh32z.png)

## Usage

1. **Prerequisites:**
   - Install VirtualBox on your host machine.
   - Download OPNsense, Kali Linux, and Windows ISO images.

2. **Virtual Network Setup:**
   - Configure VMs for OPNsense, Kali Linux, and Windows into VirtualBox.
   - Configure network settings, ensuring proper communication between VMs.
  
  ![Host only network](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700424074/screenshots2/hostonly_network_y8pl8p.png)
  
  ![Kali Adapter Setting](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700424074/screenshots2/kali_adapter_2_syawsj.png)
  
  ![OPNsense Adapter Setting](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700424221/screenshots2/OPNsense_adapter2_ni5o07.png)

3. **OPNsense Configuration:**
   - Follow the guide to deploy and configure OPNsense.
   - Customize Nmap rules as per your network requirements.

![Custom Nmap rules installed on IDS](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700424563/screenshots2/customnmap_rules_on_IDS_j5npj7.png)
    
4. **Intrusion Detection and Vulnerability Assessments:**
   - Execute Suricata tests for intrusion detection.
   - Perform vulnerability assessments using tools available in Kali Linux.

5. **Monitoring and Log Analysis:**
   - Monitor network activities using OPNsense logs.
   - Analyze logs for potential security threats.

## Future Plans

1. **Wazuh SIEM Integration:**
   - Integrate Wazuh Security Information and Event Management (SIEM) for centralized log analysis and threat detection.

2. **XDR Agent Implementation:**
   - Implement Extended Detection and Response (XDR) agents to enhance threat detection capabilities across the network.

3. **Cortex and MISP Integration:**
   - Integrate Cortex and MISP for threat intelligence sharing and automated incident response.

4. **The Hive Integration:**
   - Incorporate The Hive for collaborative and centralized incident management and response.

5. **ZenArmor NGFW Integration:**
   - Integrate ZenArmor Next-Generation Firewall (NGFW) using syslog for enhanced network security.

6. **Deep Dive into OPNsense Firewall:**
   - Explore advanced features of the OPNsense firewall to strengthen network security measures.

7. **Proxy Configuration:**
   - Deepen the configuration of proxy services to control and monitor internet access more effectively.

8. **PFsync Configuration:**
   - Enhance the PFsync configuration to achieve high availability and synchronization between OPNsense instances.

## License

This project is licensed under the [MIT License](LICENSE.txt).
