DDoS 高防  IP（境外企业版）为已接入防护的网站业务提供 CC 频率限制防护策略，支持限制源 IP 的访问频率。频率控制防护开启后自动生效，默认使用超级宽松防护模式，频率控制防护提供多种防护模式，供您在不同场景下调整使用。您也可以自定义频率限制规则，检测到单一源 IP 在短期内异常频繁地访问某个页面时，将设置人机校验或丢弃策略。

频率控制防护提供不同的防护模式，允许您根据网站的实时流量异常调整频率控制策略，具体包括如下模式：
<dx-tabs>
::: 宽松等级
此等级下的 CC 防护策略较为宽松，可能会存在少部分异常请求透传的风险。注意：当发生攻击时，可切换防护等级进行防护。也可以配置自定义 CC 频率限制策略进行防护。
:::
::: 适中等级
将启动人机校验算法，访问者通过算法验证后才允许访问源站。注意：此防护等级只适用于 Web 网站业务，不适用于 API/APP 类业务。如果为 API/APP 类业务，请配置自定义 CC 频率限制策略进行防护。
攻击紧急：当发现源站访问量突然增加，导致源站服务器负载过高或者响应异常时，可选择此等级进行防护。
:::
::: 严格等级
针对全网每一个访问者都会进行人机识别验证，同时验证算法升级，认证过程更加严格，可能会存在一定误杀。注意：此防护等级只适用于 Web 网站业务，不适用于 API/APP 类业务。如果为 API/APP 类业务，请配置自定义 CC 频率限制策略进行防护。
:::
:::攻击紧急
当发现源站访问量突然增加，导致源站服务器负载过高或者响应异常时，可选择此等级进行防护。
:::
::: 自定义
基于设置的自定义频控规则进行防护，针对特征符合频控规则设置条件的流量进行访问频率限制。
:::
</dx-tabs>



## 前提条件
您需要成功 [购买 DDoS 高防 IP（境外企业版）](https://cloud.tencent.com/document/product/1014/56255)  ，并设置防护对象。


## 操作步骤
1. 登录 [DDoS 高防 IP（境外企业版）](https://console.cloud.tencent.com/ddos/ddos-basic) 控制台 ，在左侧导航中，单击 **DDoS 高防 IP** > **防护配置** > **CC 防护**。
2. 在 CC 防护页面的左侧列表中，选中高防 IP 的 ID，如“bgp-00xxxxxx”。
![](https://qcloudimg.tencent-cloud.cn/raw/8dffdad7a2bb7a9cf45d59390c4597d1.png)
3. 在 CC 频率限制卡片中，单击**设置**。
4. 在 CC 频率限制列表，单击**新建**，选择或新增该 IP 下的域名，打开防护状态，选择相应的防护等级。
![](https://qcloudimg.tencent-cloud.cn/raw/55ec4068e2b631871156fb67cfdd6cbc.png)
5.	如需设置自定义规则，单击**新增规则**，创建频率限制规则，填写相关字段，单击**确定**。
![](https://qcloudimg.tencent-cloud.cn/raw/6501cf5a33080f8a2f5ec08a04fff270.png)
**参数说明：**
6. 新建完成后，在 CC 频率限制列表将新增一条 CC 频率限制规则，可以在右侧操作列单击**配置**，修改 CC 频率限制规则。
![](https://qcloudimg.tencent-cloud.cn/raw/1b6c04d65c5052287bbfab26bf9e115f.png)
