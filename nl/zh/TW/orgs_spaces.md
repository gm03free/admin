---

copyright:

  years: 2015, 2017
lastupdated: "2017-03-03"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# 管理組織和空間
{: #orgsspacesusers}

身為帳戶擁有者，您可以使用「管理組織」頁面來管理組織。組織管理員也可以使用「管理組織」頁面來管理將他們設為管理員的任何組織。
{:shortdesc}

若要管理組織及空間，請從 {{site.data.keyword.Bluemix_notm}} 功能表列按一下**管理** &gt; **帳戶** &gt; **組織**。 

**附註**：您必須是「隨收隨付制」帳戶的帳戶擁有者，才能建立組織。

## 管理組織
{: #orginfo}

組織可以跨越多個地區，而且是透過下列項目所定義：

<dl>
<dt>團隊成員</dt>
<dd>組織及空間中具有基本許可權的角色。您必須先被指派給組織，才能獲授與組織內空間的其他許可權。如需詳細資訊，請參閱[使用者及角色](/docs/admin/users_roles.html#userrolesinfo)。</dd>
<dt>網域</dt>
<dd>提供網際網路上配置給組織的路徑。路徑具有一個子網域及一個網域。子網域一般是應用程式名稱。網域可能是系統網域，或您針對應用程式所登錄的自訂網域。請參閱[管理自訂網域](/docs/admin/orgs_spaces.html#managedomains)。<br/>
<p>**附註**：如果您新增自訂網域，則必須配置 DNS 伺服器來解析自訂網域，以指向 {{site.data.keyword.Bluemix_notm}} 系統網域。使用此方式，{{site.data.keyword.Bluemix_notm}} 接到您的自訂網域的要求時，可以將它適當地遞送至您的應用程式。</p></dd>
<dt>配額</dt>
<dd>代表組織的資源限制，包括可配置供組織使用的服務數目及記憶體量。建立組織時，會指派配額。組織空間中的任何應用程式或服務都會使用配額。使用「隨收隨付制」或「訂閱」方案，您可以在組織需要變更時，調整 Cloud Foundry 應用程式及容器的配額。請參閱[管理配額](/docs/admin/orgs_spaces.html#managequota)。</dd>
</dl>

在 {{site.data.keyword.Bluemix_notm}} 中，您可以使用組織來啟用團隊成員之間的協同作業，以及使用下列方式促進專案資源的邏輯分組：

<ul>
<li>您可以將組織中的一組空間、應用程式、服務、網域、路徑及團隊成員群組在一起。</li>
<li>您可以根據每位使用者管理空間及組織的存取權。</li>
</ul>

建立組織時，組織名稱在 {{site.data.keyword.Bluemix_notm}} 內必須是唯一的。
如果另一位 {{site.data.keyword.Bluemix_notm}}「公用」、「專用」或「本端」使用者已在使用組織名稱，則您必須指定新的名稱。建立組織之後，您會自動獲指派*組織管理員* 許可權，這可讓您編輯組織名稱、新增團隊成員，以及在組織中建立或刪除空間。

您必須與 [{{site.data.keyword.Bluemix_notm}} 支援中心 ![外部鏈結圖示](../icons/launch-glyph.svg)](http://ibm.biz/bluemixsupport){: new_window} 聯絡，以刪除組織。當您要求支援團隊刪除組織時，會刪除組織內的所有空間、應用程式及服務。

可以將下列[使用者角色](/docs/admin/users_roles.html#userrolesinfo)指派給組織中的團隊成員：

<ul>
<li>組織管理員</li>
<li>組織帳單管理員</li>
<li>組織審核員</li>
</ul>

<!-- Add info on Manage infrastructure option under a space -->

## 使用空間
{: #spaceinfo}

在組織內，您可以使用空間來群組一組應用程式、服務及團隊成員。在 {{site.data.keyword.Bluemix_notm}} 中，空間關聯於特定地區。

將團隊成員新增至組織之後，即可將空間的許可權授與他們。與組織類似，空間也會有一組[使用者角色](/docs/admin/users_roles.html#userrolesinfo)，其具有指派給團隊成員的特定許可權：

<ul>
<li>空間管理員</li>
<li>空間開發人員</li>
<li>空間審核員</li>
</ul>

**附註**：團隊成員必須至少獲指派空間中的一個許可權。

## 建立組織和空間
{: #createorg}

只有具有「隨收隨付制」帳戶的帳戶擁有者才能建立組織。您可以完成下列步驟來建立組織：

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 按一下**新增組織**。
3. 輸入組織名稱。
4. 按一下**新增**。

您可以在組織中建立空間；例如，建立 *dev* 空間作為開發環境、*test*
空間作為測試環境，以及 *production* 空間作為正式作業環境。
然後，您可以建立應用程式與空間的關聯。請完成下列步驟，以建立空間：

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 識別您要新增空間的組織，然後選取**檢視詳細資料**。
4. 按一下**新增空間**。
5. 輸入空間名稱。
6. 按一下**新增**。

## 將組織重新命名
{: #orgrename}

完成下列步驟，以將您的組織重新命名：

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 識別您要編輯的組織，然後選取**檢視詳細資料**。
3. 選取**編輯組織**。
4. 選取組織標題的**編輯**。
5. 鍵入新的組織名稱。
6. 按一下**儲存**。

## 刪除現有組織或空間
{: #deleteorgs}

身為帳戶擁有者，您可以與 [{{site.data.keyword.Bluemix_notm}} 支援中心 ![外部鏈結圖示](../icons/launch-glyph.svg)](http://ibm.biz/bluemixsupport){: new_window} 聯絡，以刪除組織。

**附註**：刪除作業無法回復。您會遺失與組織相關聯的所有應用程式和服務。


您可以從**管理組織**頁面刪除空間：

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 識別您要編輯的組織，然後選取**檢視詳細資料**。
3. 識別您要刪除的空間，然後選取**編輯空間**。
4. 按一下**刪除空間**。

## 列出成員
{: #listmembers}

完成下列步驟，以列出特定組織的成員：

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 識別您要檢視其成員的組織，然後按一下**檢視詳細資料**。
3. 按一下**編輯組織**。
4. 您可以在**使用者**標籤中看到組織的成員及其角色。

完成下列步驟，以列出特定空間的成員：

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 識別您要檢視其成員的組織，然後按一下**檢視詳細資料**。
3. 識別您要檢視其成員的空間，然後按一下**編輯空間**。
4. 您可以在**使用者**標籤中看到空間的成員及其角色。

## 管理配額
{: #managequota}

身為 {{site.data.keyword.Bluemix_notm}} 帳戶擁有者或組織管理員，您可以檢視針對組織所使用及配置的配額。此配額代表建立組織時指派給組織的資源限制。根據您具有的是試用帳戶還是可入帳帳戶，組織可用的資源會不同。組織空間中的任何應用程式或服務都會影響已配置配額的使用。

若要檢視針對組織所使用及配置的配額，請完成下列步驟：

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 識別您要檢視其配額的組織，然後按一下**檢視詳細資料**。
3. 按一下**編輯組織**。
4. 如果您的空間定義在多個地區中，請選取您要檢視的特定地區。
5. 按一下**配額**。 
6. 預設會開啟 **Cloud Foundry** 配額頁面。您可以檢視下列資源的配額詳細資料：
 * 記憶體
 * 服務
 * 方案
 * 價格
7. 按一下**容器**，以檢視已使用及可用的容器配額配置。容器配置會根據定價方案而不同。您可以檢視下列資源的配額詳細資料：
 * 記憶體
 * 公用 IP
 * 檔案共用
8. 按一下**虛擬伺服器**，以檢視虛擬機器。

**附註：**{{site.data.keyword.Bluemix_notm}} 雪梨地區尚無法使用容器。 

如需容器的相關資訊，請參閱「容器」文件中的[配額](/docs/containers/container_planning_org_ov.html#container_planning_quota)。
若要變更配置給組織的配額，您必須開啟支援問題單。如需開啟支援問題單的相關資訊，請參閱[取得客戶支援](/docs/support/index.html#contacting-support)。 

## 管理網域
{: #managedomains}

身為帳戶擁有者或組織管理員，您可以檢視系統網域，以及新增在組織及其空間內建置之應用程式的自訂網域。身為空間管理員，空間的**網域**標籤是指派給空間之網域的唯讀清單。

1. 按一下**管理** &gt; **帳戶** &gt; **組織**。
2. 識別您要檢視或編輯其網域的組織。
3. 選取該組織的**檢視詳細資料**。
4. 按一下**編輯組織**。
5. 按一下**網域**。

如果您新增自訂網域，則必須配置 DNS 伺服器來解析自訂網域，以指向 {{site.data.keyword.Bluemix_notm}} 系統網域。使用此方式，{{site.data.keyword.Bluemix_notm}} 接到您的自訂網域的要求時，可以將它適當地遞送至您的應用程式。空間隨時都可以使用系統網域，也可以將自訂網域配置給空間。在空間中建立的應用程式可能會使用針對該空間所列出的任何網域。如需建立及使用自訂網域的相關資訊，請參閱[使用自訂網域](/docs/manageapps/updapps.html#domain)。