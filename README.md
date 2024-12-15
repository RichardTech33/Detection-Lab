# SIEM and Log Analysis Project with Splunk Cloud

## **Introduction**
Implement a SIEM system using Splunk to collect, analyze, and correlate security logs from devices on your home network.

## **Objectives**
- Gain hands-on experience in setting up and managing a SIEM system.
- Collect and analyze logs from various home network devices.
- Create security alerts and generate reports.

## **Skills Learned**
- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

## Step-by-Step Implementation

### 1. Splunk Cloud Setup

1. **Sign Up for Splunk Cloud**
   - Go to the [Splunk Cloud website](https://www.splunk.com/en_us/software/splunk-cloud.html) and sign up for an account.
   - Follow the prompts to set up your environment.

2. **Create an Index**
   - Navigate to the Splunk Cloud interface.
   - Go to `Settings` > `Indexes` and click `New Index`.
   - Enter a name for the index and configure any additional settings as needed.
   - <img width="700" alt="Screenshot 2024-08-01 at 8 57 36 PM" src="https://github.com/user-attachments/assets/25ddab00-56af-4a48-ab8c-ddcbabcbac36">

### 2. Forwarder Configuration

1. **Download and Install the Universal Forwarder**
   - Download the Splunk Universal Forwarder from the [Splunk Downloads page](https://www.splunk.com/en_us/download/universal-forwarder.html).
   - Install the forwarder on your home network devices.

2. **Configure the Forwarder**
   - Edit the `inputs.conf` file to specify the log sources.
   - Update the `outputs.conf` file with the Splunk Cloud instance details.

3. **Verify Forwarder Connectivity**
   - Use the `splunk btool` command to check the forwarder configuration.
   - Ensure that the forwarder is successfully sending logs to Splunk Cloud. In this instance you, can verify this information in the Splunk terminal without having to use the interface. As shown below:
   - <img width="700" alt="ForwarderCLI" src="https://github.com/user-attachments/assets/6fc3f408-fc38-46a0-91bc-903536050a59">

### 3. Log Collection

1. **Define Log Sources**
   - Identify and configure the devices and applications from which logs will be collected.
   - Ensure that each source is properly configured to forward logs.

2. **Verify Log Collection**
   - Check the Splunk Cloud interface to ensure logs are being ingested correctly.

### 4. Data Ingestion

1. **Configure Data Inputs**
   - Go to `Settings` > `Data Inputs` in Splunk Cloud.
   - Add data inputs for each log source.

2. **Monitor Data Ingestion**
   - Use Splunk’s monitoring tools to ensure logs are being collected and indexed properly.

### 5. Search and Analysis

1. **Create Search Queries**
   - Develop SPL (Search Processing Language) queries to analyze log data.
   - Save and test queries to ensure they return relevant results.
   - <img width="700" alt="Screenshot 2024-08-01 at 4 28 11 PM" src="https://github.com/user-attachments/assets/563121f9-8006-4c4e-8496-73f72108eee8">

2. **Build Dashboards**
   - Create dashboards to visualize log data and monitor key metrics.
   - Add panels for charts, graphs, and other visualizations.
   - <img width="700" alt="Dashboard Screenshot" src="https://github.com/user-attachments/assets/62afe7ae-8ccb-485d-a88b-9fa157397c51">

### 6. Alerting and Monitoring

1. **Set Up Alerts**
   - Go to `Settings` > `Searches, Reports, and Alerts`.
   - Create alerts based on specific conditions or thresholds.
   - <img width="700" alt="Splunkalert" src="https://github.com/user-attachments/assets/eb5227d7-6681-4888-9be4-9621201f3941">

2. **Configure Notification Settings**
   - Set up email or other notification methods to alert you of critical incidents.

### 7. Reporting

1. **Generate Reports**
   - Use Splunk’s reporting features to create detailed reports on log analysis and security incidents.

2. **Schedule Reports**
   - Set up scheduled reports to automate regular monitoring.

## Conclusion

This project demonstrates how to leverage Splunk Cloud for effective SIEM and log analysis. By setting up a forwarder, collecting logs, and analyzing data, you can gain valuable insights into your network’s security posture and respond to potential threats. For my specific log, there are no security events to show but one can set alerts for if/when they are to occur.

## **References and Resources**
- **Official Documentation**: [Splunk Documentation](https://docs.splunk.com/Documentation/Splunk)
- **Community Forums**: [Splunk Answers](https://community.splunk.com/)
- **Tutorials and Courses**: [Splunk Education](https://www.splunk.com/en_us/training.html)


