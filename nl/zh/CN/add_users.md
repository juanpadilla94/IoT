---

copyright:
  years: 2016, 2018
lastupdated: "2018-03-14"

---

{:new_window: target="blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# 管理用户访问权
{: #managing-user-access}

在成员仪表板中，可以控制和管理对 {{site.data.keyword.iot_full}} 组织的访问权。您可以通过添加、邀请<!--, registering-->或导入用户来添加用户。还可以通过分配角色来向用户授予不同的访问级别。
{:shortdesc}

## 添加用户
{: #adding-new-users}

在仪表板的**成员**选项卡中，可以使用“添加”功能来添加单个成员。还可以使用“导入”功能同时添加多个成员。

缺省情况下，成员帐户不会到期。向 {{site.data.keyword.iot_short_notm}} 组织添加用户时，可以选择为其帐户设置到期日期。

### 向 {{site.data.keyword.iot_short_notm}} 组织添加成员

要向组织添加成员，您将需要该成员的 IBM 标识。添加成员时，无需得到该成员的确认。

要向 {{site.data.keyword.iot_short_notm}} 组织添加单个成员，请执行以下操作：
1. 在 {{site.data.keyword.iot_short_notm}} 仪表板中，转至**成员**。
2. 单击**添加成员**，然后选择**添加**选项卡。
3. 输入成员的 IBM 标识。
4. 为成员选择角色。
5. 可选：为成员设置到期日期。
6. 单击**添加**。

要同时添加多个成员，必须上传 `.csv` 文件，此文件包含每个成员的 IBM 标识、角色和可选的到期日期。有关信息，请参阅[构造 CSV 文件](#constructing-your-csv)。
1. 在 {{site.data.keyword.iot_short_notm}} 仪表板中，转至**成员**。
2. 单击**添加成员**，然后选择**导入**选项卡。
3. 浏览文件或将 `.csv` 文件拖入**上传 CSV** 窗口中。
4. 如果无法识别 CSV 文件中指定的角色，请选择要使用的缺省角色。
5. 将 CSV 文件中的列编号映射到相应的 IBM 标识、角色和（可选）到期日期条目。
6. 选择相应的逗号或分号列分隔符，以匹配 `.csv` 文件中使用的分隔符。
7. 单击**导入**以导入 IBM 标识并创建成员。

<!--
### Inviting members to your {{site.data.keyword.iot_short_notm}} organization

When you invite a user to become a member of your {{site.data.keyword.iot_short_notm}} organization, the user receives an email that contains an invitation link. Invitation links expire 48 hours after they are sent. If an invitation link is not used within 48 hours, the user must be invited again to receive a new invitation link.

**Important:** The invite feature requires a configured mail service. For more information, see the Email section of the [External service integrations](reference/extensions/index.html#email) topic.

To invite a member to your {{site.data.keyword.iot_short_notm}} organization:
1. In the {{site.data.keyword.iot_short_notm}} dashboard, go to **Members**.
2. Select the **Invitations** tab.
2. Click **Invite Members** and select the **Invite** tab.
3. Enter the email address of the member.
4. Select a role for this member.
5. Optional: Set an expiry date for the member.
6. Click **Invite Member**.

To invite multiple members simultaneously, you must upload a `.csv` file that contains the email address, role and the optional expiry date of each member. For information, see [Constructing your CSV file](#constructing-your-csv).
1. In the {{site.data.keyword.iot_short_notm}} dashboard, go to **Members**.
2. Select the **Invitations** tab.
2. Click **Invite Members** and select the **Import** tab.
3. Browse your files or drag the `.csv` file into the **Upload CSV** window.
4. Select a default role to use if a role specified in the CSV file is not recognized.
5. Map the column numbers in your CSV file to the corresponding email address, role, and (optional) expiry date entries.
6. Select the appropriate comma or semicolon column separator to match the separator used in your `.csv` file.
7. Click **Import** to send out the invitations. -->

<!-- ### Registering a member with your {{site.data.keyword.iot_short_notm}} organization

If your organization is using {{site.data.keyword.Bluemix_notm}} {{site.data.keyword.ssoshort}}, you can add individual members to your organization by registering them, which does not require an IBMid.

To register a member with your {{site.data.keyword.iot_short_notm}} organization:
1. In the {{site.data.keyword.iot_short_notm}} dashboard, go to **Members**.
2. Select the **Invitations** tab.
2. Click **Invite Members** and select **Invite**.
3. Enter the email address of the member.
4. Select a role for this member.
5. Enter the subject, realm name, and issuer.
   **Important:** Ensure that the `Subject`, `Realm Name`, and `Issuer` fields comply with the OpenID Connect recommendations and standards. For more information, see the [OpenID Connect ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://openid.net/connect/){: new_window} website.
6. Optional: Set an expiry date for the member.
7. Click **Register Member**.

To register multiple members simultaneously, you must upload a CSV (`.csv`) file that contains the email address, role, subject, realm name, issuer, and the optional expiry date of each member.
1. In the {{site.data.keyword.iot_short_notm}} dashboard, go to **Access**.
2. Click **Add Member** and select **Import**.
3. Click **Bulk Register**.
4. Select a default role and ensure that the column numbers on your CSV file match the column numbers in the CSV settings.
5. Ensure the column separator in your CSV file matches the column separator in the CSV settings.
6. Click **Browse your files** or drag the CSV file into the **Upload CSV** window. -->

### 构造 CSV 文件
{: #constructing-your-csv}

构造用于将成员导入组织中的 CSV 文件时，确保包含所用方法的必需信息。请使用逗号或分号来分隔列。  
**重要信息：**上传 CSV 文件时，确保在 **CSV 设置**下选择正确的列分隔符。

以逗号分隔的样本 CSV 文件：  
```
user1@sample.com,PD_DEVELOPER_USER,2018-03-13
user2@sample.com,PD_OPERATOR_USER,2018-03-13
user3@sample.com,PD_ADMIN_USER,2018-03-13
```
在使用以下列条目的位置：  
- 列 1：用户的电子邮件地址。  
如果您在添加成员，请确保使用对应于有效 IBM 标识的电子邮件地址。如果您在邀请成员，那么您可以使用任何有效电子邮件地址。
- 列 2：要分配给用户的角色。  
输入以下其中一个角色：
 - PD_ADMIN_USER
 - PD_OPERATOR_USER
 - PD_DEVELOPER_USER
 - PD_ANALYST_USER
 - PD_READER_USER  
有关用户角色的更多信息，请参阅[用户、应用程序和网关角色](roles_index.html#user_roles)。
- 列 3 ：对应于用户到期日期的 ISO 6801 日期（例如 `2018-03-13`）。

## 编辑用户
{: #editing-users}

可以对用户进行编辑，以更改其角色，添加、除去或更改访问权到期日期，或者添加或除去对组织的访问权。

1. 在 {{site.data.keyword.iot_short_notm}} 仪表板左侧的导航栏中，单击**成员**。
2. 单击要编辑的用户旁的**编辑**图标。
3. 对用户进行所需的更改。
4. 单击**保存**。

## 阻止用户访问
{: #blocking-users}

可以阻止用户访问 {{site.data.keyword.iot_short_notm}} 组织，同时仍保留其组织成员资格。

1. 在 {{site.data.keyword.iot_short_notm}} 仪表板左侧的导航栏中，单击**成员**。
2. 单击要阻止其访问 {{site.data.keyword.iot_short_notm}} 组织的用户旁的切换开关。

## 限制用户访问权
{: #limiting-users}

资源级别的访问控制使您能够限制对组织内设备的访问权。您可以使用资源组来指定每个用户或 API 密钥可管理的设备。有关如何配置资源级别访问控制的信息，请参阅[配置资源级别访问控制](reference/rlac.html#configure_RLAC)。

## 除去用户
{: #removing-users}

可以从 {{site.data.keyword.iot_short_notm}} 组织中完全除去用户。除去用户的操作不可撤销，要恢复已除去用户的访问权，必须将相应用户[添加到平台](#adding-new-users)。

1. 在 {{site.data.keyword.iot_short_notm}} 仪表板左侧的导航栏中，单击**成员**。
2. 单击要除去的用户旁的**删除**图标。
3. 单击确认对话框中的**删除**。
