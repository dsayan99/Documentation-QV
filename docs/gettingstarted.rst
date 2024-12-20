Getting Started
===============

Getting Started with QCapture
-----------------------------

This section guides you through the initial steps to use QCapture for
preprocessing network traffic and uploading cryptographic data to the
QVision Dashboard.

Accessing QCapture
------------------

1. Open a web browser and navigate to QCapture's URL:

http://<vm-ip-address>:8501

Replace <vm-ip-address> with the IP address of the virtual machine where
QCapture is installed.

2. You will see the **QVision Uploader** interface, as shown below:

.. figure:: media/image1.png
   :alt: A screenshot of a computer Description automatically generated
   :width: 6.26389in
   :height: 3.52361in

   A screenshot of a computer Description automatically generated

Uploading and Analyzing PCAP Files
----------------------------------

1. **Enter Organization Unit ID**:

   -  Specify a unique identifier for the Organization where the PCAP
      files originate. This helps in organizing data by organization.

2. **Enter Network Unit ID**:

   -  Specify a unique identifier for the network unit where the PCAP
      files originate. This helps in organizing data by network
      segments.

3. **Enter a Scan Name**:

   -  Provide a meaningful name for the scan. This can represent the
      scope or purpose of the analysis (e.g., "Firewall Traffic - Dec
      2024").

4. **Choose Files to Upload**:

   -  Drag and drop the PCAP files into the designated area or click
      **Browse Files** to select files from your local system.

   -  Note: Ensure each file is under the size limit of 200 MB.

5. **Upload Files**:

   -  After adding the files, click the **Upload Files** button.

   -  QCapture will process the PCAP files, extract cryptographic data
      (algorithms, certificates, and protocols), and automatically
      upload the results to the QVision Dashboard.

Verifying the Upload
--------------------

-  Once the analysis is complete, log in to the QVision Dashboard to
   review the processed cryptographic logs and compliance data.

Getting Started with QVision Dashboard
--------------------------------------

This section provides a step-by-step guide to begin using the QVision
Dashboard for managing cryptographic compliance and inventory.

**QVision Home:**

1. Home

   2. Manage Users

**Organization Dashboard:**

   1. Organization Overview

   2. Cryptographic Inventory

   3. Manage Network Units

   4. Manage Certificate Authorities

   5. Mange Policies

**Network Unit Dashboard:**

   1. NU Overview

   2. Cryptographic Inventory

   3. Manage Audits

**Audit Dashboard:**

   1. Audit Overview

   2. Manage Audit Data

   3. Cryptographic Inventory

   4. Manage Mapping

   5. Discover Connections

   6. Inventory

   7. Policy Compliance

QVision Home: Home Tab
----------------------

The **Home** tab in QVision Home serves as the primary interface for
managing organizations and monitoring compliance scores.

1. **Enroll a New Organization** (Admin Only)

   -  Admin users can create new organizations using the **Create New
      Organization** button.

   -  Clicking this button opens a form with the following fields:

      -  **Organization Name**: The name of the organization.

      -  **Type of Organization**: Select the type (e.g., Government,
         Enterprise).

      -  **Sector of Organization**: Choose the sector (e.g.,
         Healthcare, Finance).

      -  **Contact Person Name**: Enter the name of the primary contact.

      -  **Email ID of Contact Person**: Provide the email address of
         the contact.

   -  After filling in the form, click **Enroll Organization** to add
      the organization to the system.

2. **List of Organizations**

   -  The page displays all enrolled organizations in a card format.

   -  Each organization card includes:

      -  **Organization Name**

      -  **Organization ID**

      -  **Type and Sector**

      -  **Last Audit Date**

      -  **Cryptography Health Score**: Displays the overall compliance
         score and health status.

      -  **Policy Status**: Highlights compliance results for policies
         (e.g., Compliant, No Critical Issues Found, Critical Issues
         Found).

3. **Navigate to Organization Dashboard**

   -  To view detailed information about an organization, click on the
      **Org. Dashboard** button on the respective organization card.
      This action will take you to the organization’s dashboard, where
      you can dive deeper into its cryptographic inventory and
      compliance data.

QVision Home: Manage Users Tab
------------------------------

The **Manage Users** tab in QVision Home allows administrators to manage
user accounts, including adding new users, editing existing user
details, and removing users. It also provides an overview of user roles
and responsibilities across enrolled organizations.

1. **User List**:

   -  Displays all registered users along with their details, including:

      -  **User Name**

      -  **User ID**

      -  **Email Address**

      -  **Designation**

      -  **Roles and Responsibilities** for each organization (e.g.,
         Owner, Auditor, Viewer).

2. **Add New User**:

   -  To enroll a new user:

      -  Click the **Create New User** button.

      -  Fill out the form with the following details:

         -  **User Name**: Enter the name of the user.

         -  **Email ID**: Provide the user’s email address.

         -  **Password**: Set a secure password for the user.

         -  **Designation**: Specify the user’s role or position.

         -  **Assign Role to User**: Assign specific roles for each
            enrolled organization (Owner, Auditor, Viewer).

      -  Click **Create New** to save the user.

3. **Edit User Details**:

   -  To edit user information:

      -  Click the **Edit** icon next to the user’s name.

      -  Update the relevant details using the same form used for
         creating a user.

      -  Save changes.

4. **Delete User**:

   -  To remove a user:

      -  Click the **Delete** icon next to the user’s name.

      -  Confirm the deletion action to remove the user from the system.

Organization Dashboard: Organization Snapshot
---------------------------------------------

The **Organization Overview** section provides detailed information
about a specific organization, along with a visual representation of its
compliance with different policies.

1. **Organization Details**:

   -  Displays key information about the organization, including:

      -  **Organization Name**: The registered name of the organization.

      -  **Organization ID**: A unique identifier for the organization.

      -  **Type of Organization**: Classification of the organization
         (e.g., Government, Enterprise).

      -  **Type of Networks**: The network type managed by the
         organization (e.g., Public Facing Network).

      -  **Number of Network Units**: Total network units within the
         organization.

      -  **Most Recent Audit**: Date of the latest audit conducted for
         the organization.

      -  **Contact Details**: Includes the name, email, and designation
         of the primary contact.

      -  **Created By**: Indicates the user who enrolled the
         organization.

      -  **Creation Date**: Date when the organization was added to the
         system.

2. **Policy Compliance Overview**:

   -  A graphical representation categorizing policy compliance into
      **High**, **Medium**, and **Low** risk levels.

   -  Allows users to:

      -  Filter compliance data by selecting a specific policy from the
         dropdown menu.

      -  View compliance trends over a defined time range using the date
         picker.

3. **Edit Organization Details**:

   -  Click the **Edit** button to update the organization's
      information.

Organization Dashboard: Cryptographic Inventory
-----------------------------------------------

The **Cryptographic Inventory** section provides a visual representation
of cryptographic data for a specific organization. This section features
interactive pie charts to help users analyze key parameters related to
connections, algorithms, and certificates. This section offers a
high-level overview of the cryptographic practices within an
organization, enabling users to identify trends, gaps, or potential
risks in their inventory.

1. **Connections:**

   -  **Displays pie charts summarizing:**

      -  **Protocols of Connections:** Breakdown of connection protocols
         (e.g., TLS 1.2, SSL 1.3) by usage count.

      -  **Security of Connections:** Categorization of connections
         based on their security levels.

2. **Algorithms:**

   -  **Features charts representing the usage of cryptographic
      algorithms, including:**

      -  **Encryption Methods:** Proportion of encryption algorithms
         used (e.g., RSA, ECC, AES).

      -  **Decryption Methods:** Summary of algorithms used for
         decryption.

3. **Certificates:**

   -  *(Details for certificate-related charts can be added based on
      additional inputs.)*

4. **Filters:**

   -  Use the Pick a Date filter to narrow down the data to a specific
      time range, allowing users to track changes and trends over time.

Organization Dashboard: Manage Network Units
--------------------------------------------

The **Manage Network Units** section provides an overview of all network
units within an organization, displaying key details and compliance data
for each unit.

1. **Network Unit List**:

   -  Displays a list of all network units associated with the
      organization.

   -  Each unit card includes:

      -  **Network Unit Name**: The name of the network unit.

      -  **Network Unit ID**: A unique identifier for the network unit.

      -  **Network Type**: Classification of the network (e.g.,
         Government, Enterprise).

      -  **Created By**: Indicates who created the network unit entry.

      -  **Created On**: Date of creation.

      -  **Last Audit Date**: When the unit was last audited.

2. **Cryptography Health Score**:

   -  Provides a health score for each network unit, categorized as:

      -  **A**: Excellent compliance.

      -  **B**: Good compliance (some minor issues).

      -  **C**: Needs improvement.

      -  **D**: Critical issues.

3. **Policy Compliance**:

   -  Displays the status of each policy applied to the network unit:

      -  **Compliant**

      -  **No Critical Issues Found**

      -  **Critical Issues Found**

4. **Create New Network Unit** (Admin Only):

   -  Click **Create New** to add a new network unit.

   -  Enter relevant details (e.g., name, type, and associated
      organization).

5. **Edit or Delete Network Units**:

   -  Use the **Edit** icon to update the details of a network unit.

   -  Click the **Delete** icon to remove a network unit.

6. **Access Network Unit Dashboard**:

   -  Click **NU Dashboard** to view a detailed dashboard for a specific
      network unit.

Organization Dashboard: Manage Certificate Authorities (CAs)
------------------------------------------------------------

The **Manage Certificate Authorities (CAs)** section enables users to
manage trusted certificate authorities associated with an organization.
It provides options to view, add, and remove CA details, ensuring secure
cryptographic operations within the network. This section ensures secure
management of certificate authorities, supporting the organization in
maintaining a robust cryptographic infrastructure.

1. **Certificate Authority List**:

   -  Displays all trusted CAs associated with the organization in a
      table format.

   -  Each row includes the following details:

      -  **Trusted CA ID**: Unique identifier for the certificate
         authority.

      -  **Common Name**: The name of the certificate authority.

      -  **Organization**: The organization associated with the CA.

      -  **Organization Unit**: Specific unit within the organization
         (if applicable).

      -  **Locality**: The location of the certificate authority.

      -  **Site/Province**: Province or state of the CA.

      -  **Country**: Country of the CA.

2. **Add Certificate Authorities**:

   -  Users can add new CAs using one of the following methods:

      -  **Manually Enter CA Details**: Fill in the required details in
         a form:

         -  **Common Name**

         -  **Organization**

         -  **Organization Unit**

         -  **Locality**

         -  **State/Province**

         -  **Country**

      -  **Upload CA Certificate**: Upload a CA certificate file to
         automatically populate the details.

3. **Delete Certificate Authorities**:

   -  Remove a CA entry by clicking the **Delete** icon in the
      **Actions** column of the table.

.. **Organization Dashboard: Manage Policies**

Network Unit Dashboard: Network Unit Overview
---------------------------------------------

The Network Unit Overview section provides detailed information about a
specific network unit, including its general details and a visual trend
analysis of issues detected across multiple audits. This section
provides a comprehensive overview of the network unit's status and
allows users to track improvements or deteriorations in cryptographic
compliance over time.

1. **Network Unit Details:**

   -  Displays key information about the network unit, such as:

      -  **Network Unit Name:** The name assigned to the network unit.

      -  **Network Unit ID:** A unique identifier for the unit.

      -  **Network Type:** Classification of the network (e.g.,
         Government, Public Facing Network).

      -  **Created By:** The user or entity responsible for creating the
         network unit entry.

      -  **Created On:** The date the network unit was added to the
         system.

      -  **Last Audit Date:** The date of the most recent audit
         performed on the network unit.

2. **Issue Trend Analysis:**

   -  A graphical representation of issues categorized by severity
      (High, Medium, and Low).

   -  Displays how issues have evolved over time and across multiple
      audits.

   -  Users can filter data by:

      -  **Severity:** Select a specific severity to view its trend.

      -  **Date Range:** Use the date picker to narrow down the analysis
         to a specific time frame.

3. **Edit Network Unit:**

   -  Click the Edit button to update the network unit's details.

Network Unit Dashboard: Cryptographic Inventory
-----------------------------------------------

The Cryptographic Inventory section within the Network Unit Dashboard
provides an in-depth analysis of cryptographic data associated with a
specific network unit. This section visualizes key parameters using
interactive pie charts to facilitate effective monitoring and
decision-making.

1. **Connections:**

   -  Displays pie charts summarizing:

      -  **Protocols of Connections:** Breakdown of protocols (e.g., TLS
         1.1, TLS 1.2, SSL 1.3) based on their usage counts.

      -  **Security of Connections:** Categorization of connections by
         their security levels (e.g., high, medium, low).

2. **Algorithms:**

   -  Visualizes the usage of cryptographic algorithms in the network
      unit:

      -  **Encryption Methods:** Proportion of algorithms used for
         encryption (e.g., RSA, ECC, AES).

      -  **Decryption Methods:** Overview of algorithms used for
         decryption tasks.

3. **Certificates:**

   -  *(Details for certificate-related data will be included based on
      further input.)*

4. **Date Filter:**

   -  Utilize the Pick a Date filter to analyze data over a specific
      time period, enabling users to observe trends and shifts in
      cryptographic practices.

This section empowers users to assess the cryptographic posture of a
network unit, identify vulnerabilities, and ensure compliance with
relevant policies.

Network Unit Dashboard: Manage Audits
-------------------------------------

The **Manage Audits** section provides functionality to create new
audits and review the history of audits conducted on a specific network
unit. This section ensures efficient tracking and management of audit
data for cryptographic compliance. This section enables users to
maintain an organized and thorough audit history, ensuring transparency
and compliance with cryptographic policies.

1. **Create a New Audit**:

   -  Click the **Create New** button to initiate a new audit.

   -  A form will open requiring the following details:

      -  **Audit Name**: Provide a meaningful name for the audit.

      -  **Policy**: Select the applicable policy from the dropdown
         menu.

      -  **Upload Cryptographic Logs**: Upload cryptographic logs that
         were preprocessed by the QCapture component.

         -  You can upload the relevant certificate files or logs by
            clicking **Upload File**.

   -  Once the details are filled in, click **Start Audit** to begin the
      audit process.

2. **Audit History**:

   -  Displays a list of previously conducted audits on the network
      unit.

   -  Each audit card includes:

      -  **Audit ID**: A unique identifier for the audit.

      -  **Date & Time**: The timestamp of when the audit was conducted.

      -  **Auditor ID**: The identifier for the auditor or audit type
         (e.g., Financial Audit).

      -  **Policy Used**: The cryptographic policy applied during the
         audit.

      -  **Compliance Grade**: The overall compliance score (e.g., Grade
         A).

      -  **Issue Severity**:

         -  **Critical Issues**: Number of high-severity issues
            detected.

         -  **Minor Issues**: Number of medium- and low-severity issues
            detected.

   -  Provides a summary of findings categorized into:

      -  **High Severity**

      -  **Medium Severity**

      -  **Low Severity**

      -  **Positive Signals**

      -  **Informational Findings**

3. **View Audit Details**:

   -  Click the **View Audit** button on any audit card to see a
      detailed breakdown of its findings.

Audit Dashboard: Audit Overview
-------------------------------

The **Audit Overview** section provides a detailed summary of a specific
audit, highlighting key findings, compliance results, and issue
severity. This section helps users assess the results of an audit and
identify critical areas of improvement.

1. **Audit Details**:

   -  Displays key audit information, including:

      -  **Audit ID**: Unique identifier for the audit.

      -  **Date & Time**: When the audit was conducted.

      -  **Auditor ID**: Indicates the type of audit (e.g., Financial
         Audit).

      -  **Policy Used**: The cryptographic policy applied during the
         audit.

2. **Compliance Summary**:

   -  Provides the overall compliance grade for the audit (e.g., Grade
      A, B, etc.).

   -  Highlights the total number of:

      -  **Critical Issues**: High-severity vulnerabilities that require
         immediate attention.

      -  **Minor Issues**: Medium- or low-severity issues that may not
         pose immediate threats but need resolution.

3. **Issue Severity Breakdown**:

   -  Categorizes audit findings into the following categories:

      -  **High Severity**: Issues with severe security implications
         (e.g., SSL/TLS service supports weak protocols).

      -  **Medium Severity**: Issues with moderate security impact
         (e.g., certificate lifetime exceeds best practices).

      -  **Low Severity**: Minor vulnerabilities that may not
         significantly impact security.

      -  **Positive Signals**: Aspects of the network found to be secure
         and well-configured.

      -  **Informational Findings**: Observations that do not
         necessarily indicate vulnerabilities but are noteworthy.

This section provides a concise and actionable summary of audit
findings, enabling users to prioritize and address vulnerabilities
effectively.

Audit Dashboard: Cryptographic Inventory
----------------------------------------

The Cryptographic Inventory section within the Audit Dashboard provides
a detailed visual representation of cryptographic data gathered during
an audit. This section utilizes pie charts to highlight key parameters,
offering a clear and concise overview of cryptographic configurations.
This section provides a comprehensive snapshot of the cryptographic
posture for the audited environment, enabling users to identify
strengths and vulnerabilities in cryptographic practices.

1. **Connections:**

   -  Displays pie charts summarizing:

      -  **Protocols of Connections:** Breakdown of protocols (e.g., TLS
         1.1, TLS 1.3, SSL 1.4) based on their usage count.

      -  **Security of Connections:** Categorization of connections by
         their security levels (e.g., SSL 1.1, SSL 1.2).

2. **Algorithms:**

   -  Visualizes the usage of cryptographic algorithms in the audited
      environment:

      -  **Encryption Methods:** Proportion of algorithms used for
         encryption (e.g., RSA, ECC, AES).

      -  **Decryption Methods:** Overview of algorithms used for
         decryption.

3. **Certificates:**

   -  *(Details for certificate-related data can be included based on
      further input.)*
