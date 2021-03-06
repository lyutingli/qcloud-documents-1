## 1 短信发送错误码
<table style="word-break:break-all; word-wrap:break-all;">
<thead><tr><th style="width:15%;">错误码</th><th style="width:45%;">原因</th><th style="width:35%;">解决方案</th></tr></thead>
  <tbody>
<tr><td>1001</td><td>sig校验失败</td><td>请核对API的sig格式说明</td></tr>
<tr><td>1002</td><td>短信/语音内容中含有敏感词</td><td>应答包会返回该敏感词，请去掉该敏感词后重新发送</td></tr>
<tr><td>1003</td><td>请求包体没有sig字段或sig为空</td><td>请遵守API接口说明规范</td></tr>
<tr><td>1004</td><td>请求包解析失败，通常情况下是由于没有遵守API接口说明规范导致的</td><td>可参考<a href="/doc/product/382/3772#11-1004.E9.94.99.E8.AF.AF.E8.AF.A6.E8.A7.A3">1004错误详解</a></td></tr>
<tr><td>1006</td><td>请求没有权限，比如没有扩展码权限等</td><td>请查看错误提示语说明，如还有问题请提供失败手机号联系<a href="/doc/product/382/3773">sms helper</a></td></tr>
<tr><td>1007</td><td>其他错误</td><td>请查看错误提示语说明，如还有问题请提供失败手机号联系<a href="/doc/product/382/3773">sms helper</a></td></tr>
<tr><td>1008</td><td>请求下发短信/语音超时</td><td>出现概率很低，可重试解决</td></tr>
<tr><td>1009</td><td>请求ip不在白名单中</td><td>您配置了校验请求来源ip，但是检测到当前请求ip不在配置列表中，如有需要请联系<a href="/doc/product/382/3773">sms helper</a></td></tr>
<tr><td>1011</td><td>不存在该REST API接口</td><td>请核查REST API接口说明</td></tr>
<tr><td>1012</td><td>签名格式错误或者签名未审批</td><td>签名只能由中英文、数字组成，要求2~8个字;如果符合签名格式规范，请核查签名是否已审批</td></tr>
<tr><td>1013</td><td>下发短信/语音命中了频率限制策略</td><td>可自行到控制台调整短信频率限制策略；语音如有需要请联系<a href="/doc/product/382/3773">sms helper</a></td></tr>
<tr><td>1014</td><td>模版未审批或请求的内容与审核通过的模版内容不匹配</td><td>可参考<a href="/doc/product/382/3772#12-1014.E9.94.99.E8.AF.AF.E8.AF.A6.E8.A7.A3">1014错误详解</a></td></tr>
<tr><td>1015</td><td>手机号在黑名单库中,通常是用户退订或者命中运营商黑名单导致的</td><td>可联系<a href="/doc/product/382/3773">sms helper</a>解决</td></tr>
<tr><td>1016</td><td>手机号格式错误</td><td>请核查下发短信/语音的用户手机号格式是否正确</td></tr>
<tr><td>1017</td><td>请求的短信内容太长</td><td><a href="/doc/product/382/3772#2-.E7.9F.AD.E4.BF.A1.E9.95.BF.E5.BA.A6">短信内容长度</a>超过限制，请调整短信长度</td></tr>
<tr><td>1018</td><td>语音验证码格式错误</td><td>请遵守API接口说明规范</td></tr>
<tr><td>1019</td><td>sdkappid不存在</td><td></td></tr>
<tr><td>1020</td><td>sdkappid已禁用</td><td>此sdkappid禁止提供服务，如有需要请联系<a href="/doc/product/382/3773">sms helper</a></td></tr>
<tr><td>1021</td><td>请求发起时间不正常，通常是由于您的服务器时间与腾讯云服务器时间差异超过10分钟导致的</td><td>请核对服务器时间及API接口中的时间字段是否正常</td></tr>
<tr><td>1022</td><td>业务短信日下发条数超过设定的上限</td><td>可自行到控制台调整短信频率限制策略</td></tr>
<tr><td>1023</td><td>单个手机号30秒内下发短信条数超过设定的上限</td><td>可自行到控制台调整短信频率限制策略</td></tr>
<tr><td>1024</td><td>单个手机号1小时内下发短信条数超过设定的上限</td><td>可自行到控制台调整短信频率限制策略</td></tr>
<tr><td>1025</td><td>单个手机号日下发短信条数超过设定的上限</td><td>可自行到控制台调整短信频率限制策略</td></tr>
<tr><td>1026</td><td>单个手机号下发相同内容超过设定的上限</td><td>可自行到控制台调整短信频率限制策略</td></tr>
<tr><td>1029</td><td>营销短信发送时间限制</td><td>查看<a href="/doc/product/382/9557#5-.E8.90.A5.E9.94.80.E7.9F.AD.E4.BF.A1.E8.A7.84.E8.8C.83">营销短信发送时间段</a></td></tr>
<tr><td>1030</td><td>不支持该请求</td><td></td></tr>
<tr><td>1031</td><td>套餐包余额不足</td><td>请<a href="https://buy.cloud.tencent.com/sms">购买套餐包</a></td></tr>
<tr><td>1032</td><td>个人用户没有发营销短信的权限</td><td></td></tr>
<tr><td>1033</td><td>欠费被停止服务</td><td>可自行登录腾讯云充值来缴清欠款</td></tr>
</table>

## 2 状态回执错误码
<table style="word-break:break-all; word-wrap:break-all;">
<thead><tr><th style="width:15%;">代码</th><th style="width:10%;">分类</th><th style="width:35%;">原因</th><th style="width:35%;">解决方案</th></tr></thead>
  <tbody>
    <tr><td>DELIVRD</td><td>三网</td><td>用户短信接收成功</td><td>无</td></tr>
    <tr><td>UNDELIVRD</td><td>三网</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MX:0003</td><td>三网</td><td>单个手机号码当天下行条数超过上限</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>解除限制</td></tr>
    <tr><td>REJECTD</td><td>三网</td><td>短消息因某种原因被拒绝</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MX:0012</td><td>三网</td><td>目标号码在客户退订黑名单中</td><td>用户回复上行退订信息后加黑的，请联系<a href="/doc/product/382/3773">sms helper</a>解除黑名单</td></tr>
    <tr><td>MX:0011</td><td>三网</td><td>目标号码在禁1年黑名单中</td><td>禁1年黑名单中的号码均为恶意投诉号码，或是多次投诉的高危号码</td></tr>
    <tr><td>BWLIST _006</td><td>三网</td><td>网关黑名单</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>沟通解决</td></tr>
    <tr><td>TE:0003</td><td>三网</td><td>单个手机号码当天下行条数超过上限</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>解除限制</td></tr>
    <tr><td>TE:0014</td><td>三网</td><td>人工审核不通过</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>沟通</td></tr>
    <tr><td>TE:0002</td><td>三网</td><td>向网关提交短信失败</td><td>无</td></tr>
    <tr><td>TD:0001</td><td>三网</td><td>网关黑名单</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>沟通解决</td></tr>
    <tr><td>TD:0004</td><td>三网</td><td>疑似钓鱼，请核实</td><td></td></tr>
    <tr><td>TD:19</td><td>三网</td><td>黑名单号码</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>沟通解决</td></tr>
    <tr><td>TD:18</td><td>三网</td><td>未知运营商号码</td><td>无</td></tr>
    <tr><td>UNDELIV</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0013</td><td>移动</td><td>停机或关机</td><td>无</td></tr>
    <tr><td>MN:0001</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MK:0012</td><td>移动</td><td>空号</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MK:0005</td><td>移动</td><td>该短消息的被叫用户的开户数据的21号增值业务属性是否支持</td><td>如号码状态正常，可请用户自行拨打当地运营商客服电话确认手机端短信业务是否开启</td></tr>
    <tr><td>MK:0005</td><td>移动</td><td>呼叫被禁止。该用户的短消息业务被禁止了。在维测台中的错误值为5。在ETSI GSM 0902协议中定义为13。</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MK:0000</td><td>移动</td><td>号码为空号</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0054</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MK:0001</td><td>移动</td><td>MK0001是HLR查无此号，短信中心返回状态为无法识别被叫号码。说明用户发送的号码有误</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED</td><td>移动</td><td>短消息超过有效期</td><td>手机终端长时间未响应，导致短信接收失败</td></tr>
    <tr><td>MI:0024</td><td>移动</td><td>停机或关机</td><td>无</td></tr>
    <tr><td>MI:0011</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MC:0151</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>IC:0001</td><td>移动</td><td>停机或关机</td><td>无</td></tr>
    <tr><td>MI:0029</td><td>移动</td><td>停机或关机</td><td>无</td></tr>
    <tr><td>MI:0005</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MK:0004</td><td>移动</td><td>停机或关机</td><td>无</td></tr>
    <tr><td>MI:0000</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MI:0022</td><td>移动</td><td>移动网关的内部错误</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>IA:0054</td><td>移动</td><td>超时未接收到响应消息</td><td>请核实手机终端是否处于正常状态，可请用户重启手机后再次测试看看</td></tr>
    <tr><td>MC:0055</td><td>移动</td><td>由于用户不在服务区或内存满导致发送失败</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0059</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0036</td><td>移动</td><td>用户当时不在服务区</td><td>请核实手机终端是否处于正常状态，主要为用户端忙碌导致短信下发失败</td></tr>
    <tr><td>MI:0004</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MI:0020</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MK:0029</td><td>移动</td><td>暂时无法接通</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0084</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MK:0024</td><td>移动</td><td>下发短消息时，目的手机关机，导致该短消息下发失败。</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MK00001</td><td>移动</td><td>手机终端是空号</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0017</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MK:0015</td><td>移动</td><td>下发短消息时，手机在接收过程出现软件问题。例如，手机重启后，处理短消息部分软件没有初始化完成，此时无法正常处理短消息。</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0029</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>IC:0151</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0075</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0010</td><td>移动</td><td>暂时无法接通</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>IC:0015</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>BEYONDN</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0055</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MI:0010</td><td>移动</td><td>号码已失效</td><td>无</td></tr>
    <tr><td>MC00151</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>IC:0055</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MB:1078</td><td>移动</td><td>运营商内部错误</td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>MN00001</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>ID:0013</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MC:0001</td><td>移动</td><td>未知错误</td><td>无</td></tr>
    <tr><td>MK:0017</td><td>移动</td><td>手机内存满。</td><td>手机保存短消息的空间已满，需要清除保存的短消息，释放空间。</td></tr>
    <tr><td>MI:0081</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>DA:0054</td><td>移动</td><td>超时未接收到响应消息</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MB:1042</td><td>移动</td><td>SMC内存中缓存的、要下发给被叫用户的短消息数超过了该用户的最大下发数。</td><td>检查该被叫号码在SMC内存中的短消息积压情况。若达到了该被叫实体的最大下发数，请稍后再提交。</td></tr>
    <tr><td>ERR_NUM</td><td>移动</td><td>被叫号码不正确或被限制</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0054</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MK:0011</td><td>移动</td><td>停机或关机</td><td>无</td></tr>
    <tr><td>MN:0052</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0008</td><td>移动</td><td>用户当前所在地区信号不好，无法接收短消息。</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>IA:0073</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>IA:0051</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0075</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0022</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0020</td><td>移动</td><td>移动网关的内部错误</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI00029</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0008</td><td>移动</td><td>移动网关的内部错误</td><td>无</td></tr>
    <tr><td>MI:0012</td><td>移动</td><td>非法设备</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0012</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0059</td><td>移动</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>MN:0050</td><td>移动</td><td>空号、停机或关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0017</td><td>移动</td><td>短消息被拒绝</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0045</td><td>移动</td><td>移动网关的内部错误</td><td>无</td></tr>
    <tr><td>MN:0055</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>NOROUTE</td><td>移动</td><td>查找路由失败</td><td>无</td></tr>
    <tr><td>MI:0036</td><td>移动</td><td>移动网关的内部错误</td><td>无</td></tr>
    <tr><td>MB:1077</td><td>移动</td><td>黑名单，用户在移动公司有恶意投诉记录</td><td>需要用户自己与移动运营商10086沟通解除</td></tr>
    <tr><td>MK:0020</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0022</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MN:0053</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>DB:0505</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>ID:0070</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MX:0002</td><td>移动</td><td>向上级通道提交短信失败</td><td>无</td></tr>
    <tr><td>DB:0141</td><td>移动</td><td>曾多次投诉移动或者工信部的黑名单</td><td>无法解除</td></tr>
    <tr><td>MA:0051</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>IB:0008</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI00000</td><td>移动</td><td>消息在短信中心过期</td><td>无</td></tr>
    <tr><td>DB:0164</td><td>移动</td><td>运营商黑名单</td><td>无</td></tr>
    <tr><td>MK:0013</td><td>移动</td><td>空号</td><td>无</td></tr>
    <tr><td>DB:0144</td><td>移动</td><td>用户在全局黑名单中</td><td>无</td></tr>
    <tr><td>BWLIST</td><td>移动</td><td>网关黑名单</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>解除黑名单</td></tr>
    <tr><td>HD:19</td><td>移动</td><td>网关黑名单</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>解除黑名单</td></tr>
    <tr><td>MI00020</td><td>移动</td><td>短信下发手机终端失败ErrorinMS</td><td>无</td></tr>
    <tr><td>MI:0041</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MC:0055_006</td><td>移动</td><td>由于用户不在服务区或内存满导致发送失败</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0064</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>ERR_NUM_006</td><td>移动</td><td>被叫号码不正确或被限制</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0057</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0056</td><td>移动</td><td>响应超时</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN:0098</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0036</td><td>移动</td><td>来自MSC的未知错误。</td><td>无</td></tr>
    <tr><td>MN:0019</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0030</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0023</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0002</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0019</td><td>移动</td><td>MS不支持短消息终呼业务</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>IB:0064</td><td>移动</td><td>关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MB:1026</td><td>移动</td><td>SMC的相关运行参数（如MO速度、MT速度、短消息数、短消息实体数）已经达到了License的最大限制。</td><td>请稍后再尝试提交消息。</td></tr>
    <tr><td>MK:0055</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0066</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI00022</td><td>移动</td><td>手机终端内存满</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>IB:0009</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0006</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0053</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0023</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0045</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MC:0055_000</td><td>移动</td><td>由于用户不在服务区或内存满导致发送失败</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MA:0054</td><td>移动</td><td>运营商内部错误</td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>MK:0041</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0063</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>ID:0012</td><td>移动</td><td>计费地址错误</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MK:0084</td><td>移动</td><td>HLR返回收到未预期响应</td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>MB:0088</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI00036</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>DB00144</td><td>移动</td><td>目的号码在全局黑名单被拦截</td><td>无</td></tr>
    <tr><td>MA:0073</td><td>移动</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>MI:0099</td><td>移动</td><td>vmsc返回收到未预期响应</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0089</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0063</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0090</td><td>移动</td><td>vmsc返回远端地址不可达</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MN00013</td><td>移动</td><td>机终端停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>DB:0107</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>IB:0255</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MA:0022</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>IB:0013</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MA:0001</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0065</td><td>移动</td><td>GIW超时无应答</td><td>无</td></tr>
    <tr><td>MN:0009</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>UNKNOWN</td><td>移动</td><td>未知的短消息状态</td><td>无</td></tr>
    <tr><td>DB:0010</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0021</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0038</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MI:0052</td><td>移动</td><td>漫游限制</td><td>无</td></tr>
    <tr><td>MK:0003</td><td>移动</td><td>非法用户。本次短消息发送过程中，用户鉴权未通过，可能的原因是MSC认为该手机的鉴权密码非法。在维测台中的错误值为3。在ETSI GSM 0902协议中定义为9。</td><td>无</td></tr>
    <tr><td>MK:0009</td><td>移动</td><td>用户不在服务区MWDSET。</td><td>无</td></tr>
    <tr><td>MK:0051</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0068</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>DB:0106</td><td>移动</td><td>服务代码错误</td><td>无</td></tr>
    <tr><td>MB:1031</td><td>移动</td><td>短信中心回的，超出最大发送次数 可能是手机满了。</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MI:0048</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK00011</td><td>移动</td><td>手机终端没有短信业务"</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>MK:0048</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0056</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0057</td><td>移动</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>MK:0088</td><td>移动</td><td>vmsc返回潜在的版本不匹配</td><td>无</td></tr>
    <tr><td>TUIDING</td><td>移动</td><td>运营商黑名单</td><td>无</td></tr>
    <tr><td>HIGRISK</td><td>移动</td><td>运营商黑名单</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>解除黑名单</td></tr>
    <tr><td>CA:0054</td><td>移动</td><td>移动内部错误</td><td>无</td></tr>
    <tr><td>MN:0041</td><td>移动</td><td>当前手机处于关机、无法接通等异常状态</td><td>无</td></tr>
    <tr><td>MK:0090</td><td>移动</td><td>当前手机状态处于停机、暂时无法接通等异常状态</td><td>无</td></tr>
    <tr><td>XL:169</td><td>移动</td><td>手机号码为空号或不存在</td><td>无</td></tr>
    <tr><td>MN:xxxx</td><td>移动</td><td>M开头的移动错误代码是指Mobile，大多是因为手机端问题导致。原因有：关机，停机，信号弱，不在服务区，无效号码等等。</td><td>无</td></tr>
    <tr><td>MK:xxxx</td><td>移动</td><td>M开头的移动错误代码是指Mobile，大多是因为手机端问题导致。原因有：关机，停机，信号弱，不在服务区，无效号码等等。</td><td>无</td></tr>
    <tr><td>MI:xxxx</td><td>移动</td><td>M开头的移动错误代码是指Mobile，大多是因为手机端问题导致。原因有：关机，停机，信号弱，不在服务区，无效号码等等。</td><td>无</td></tr>
    <tr><td>TA:169</td><td>移动</td><td>空号</td><td>无</td></tr>
    <tr><td>TC:0001</td><td>移动</td><td>黑名单号码</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>沟通解决</td></tr>
    <tr><td>TC:0007</td><td>移动</td><td>短信内容涉及敏感词</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>沟通</td></tr>
    <tr><td>12</td><td>联通</td><td>计费地址错(空号、关机、停机、通话被限制或者转到联通秘书)</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>1</td><td>联通</td><td>空号、号码不存在</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>10</td><td>联通</td><td>Src_ID错(空号、关机、停机、通话被限制或者转到联通秘书)</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>24</td><td>联通</td><td>计费号码无效（用户不在使用）</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>5</td><td>联通</td><td>号码已停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>29</td><td>联通</td><td>手机用户信息错误</td><td>请确认手机号码状态是否为正确状态</td></tr>
    <tr><td>13</td><td>联通</td><td>业务代码未分配，根据MT话单里的接入号和业务代码找不到对应的申报项</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>93</td><td>联通</td><td>月租鉴权失败（用户已经停机或销户）</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>11</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>4</td><td>联通</td><td>手机关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>54</td><td>联通</td><td>用户已关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>59</td><td>联通</td><td>运营商内部错误</td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>15</td><td>联通</td><td>号码不在服务区</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>23</td><td>联通</td><td>运营商内部错误</td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>27</td><td>联通</td><td>手机不支持短消息</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>W-BLACK</td><td>联通</td><td>号码为全局黑名单</td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>解除黑名单</td></tr>
    <tr><td>17</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>51</td><td>联通</td><td>用户已关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>-37</td><td>联通</td><td>用户已关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>20</td><td>联通</td><td>暂时停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>55</td><td>联通</td><td>号码不在服务区</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>67</td><td>联通</td><td>号码是空号</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>95</td><td>联通</td><td>鉴权失败因为用户销户或不存在</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>22</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>90</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>-74</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>2</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>104</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>92</td><td>联通</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>86</td><td>联通</td><td>号码不在服务区</td><td>无</td></tr>
    <tr><td>50</td><td>联通</td><td>停机</td><td>无</td></tr>
    <tr><td>8</td><td>联通</td><td>信息长度错</td><td>无</td></tr>
    <tr><td>57</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>79</td><td>联通</td><td>内存满</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>53</td><td>联通</td><td>用户已关机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>3</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>255</td><td>联通</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>100</td><td>联通</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>61</td><td>联通</td><td>号码是空号</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>117</td><td>联通</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>45</td><td>联通</td><td>号码停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>164</td><td>联通</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>46</td><td>联通</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>14</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>9</td><td>联通</td><td>非法序列号，包括序列号重复、序列号格式错误等</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>69</td><td>联通</td><td>黑名单用户</td><td>无</td></tr>
    <tr><td>89</td><td>联通</td><td>号码不在服务区</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>64</td><td>联通</td><td>号码不在服务区</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>88</td><td>联通</td><td>号码不在服务区</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>98</td><td>联通</td><td>暂时停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>18</td><td>联通</td><td>用户未订购</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>36</td><td>联通</td><td>号码停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>44</td><td>联通</td><td>手机无短信功能</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>99</td><td>联通</td><td>暂时停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>43</td><td>联通</td><td>内存满</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>-43</td><td>联通</td><td>内存满</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>118</td><td>联通</td><td>手机无短信功能</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>52</td><td>联通</td><td>手机终端无短信接收功能</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>31</td><td>联通</td><td>非法设备</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>75</td><td>联通</td><td>号码限制</td><td>请核实手机终端是否处于正常状态，如正常可请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>103</td><td>联通</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>56</td><td>联通</td><td>欠费停机</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>106</td><td>联通</td><td>非法费用，鉴权失败</td><td>无</td></tr>
    <tr><td>-1</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>19</td><td>联通</td><td>用户未订购</td><td>无</td></tr>
    <tr><td>148</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>48</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>63</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>73</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>70</td><td>联通</td><td>号码不在服务区</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>32</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>40</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>110</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>116</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>21</td><td>联通</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>219</td><td>联通</td><td>用户手机终端处于关机、停机、暂时无法接听等不正常状态导致手机无法接收到短信</td><td>无</td></tr>
    <tr><td>182</td><td>联通</td><td>用户手机终端已暂停服务</td><td>无</td></tr>
    <tr><td>124</td><td>联通</td><td>用户手机终端处于关机、通话被限制、暂停服务等异常状态</td><td>无</td></tr>
    <tr><td>101</td><td>联通</td><td>手机号码为空号</td><td>无</td></tr>
    <tr><td>105</td><td>联通</td><td>当前手机状态处于停机、暂停服务、呼入被限制等异常情况</td><td>无</td></tr>
    <tr><td>213</td><td>联通</td><td>当前手机状态处于停机、暂停服务、呼入被限制等异常情况</td><td>无</td></tr>
    <tr><td>72</td><td>联通</td><td>145号段空号或者不存在</td><td>无</td></tr>
    <tr><td>LT:0002</td><td>联通</td><td>因信号原因导致联通失败。若批量失败则有可能是内容敏感词导致，需和运营商确认</td><td>无</td></tr>
    <tr><td>UNDELIV_601</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_602</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_640</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>REJECTD_006</td><td>电信</td><td>短消息因为某种原因被拒绝</td><td>请核实短信是否为行业短信，如是，可以请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>UNDELIV_705</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_760</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_601</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_869</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_999</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>UNDELIV_602</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_614</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_660</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_713</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>UNDELIV_615</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>EXPIRED_702</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_640</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>REJECTD_706</td><td>电信</td><td>短消息因为某种原因被拒绝</td><td>请核实短信是否为行业短信，如是，可以请用户致电联通客服确认号码的短信业务是否开通</td></tr>
    <tr><td>EXPIRED_615</td><td>电信</td><td>短消息因为某种原因被拒绝</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_765</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>UNDELIV_870</td><td>电信</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>UNDELIV_899</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>EXPIRED_001</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>UNDELIV_612</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>UNDELIV_714</td><td>电信</td><td></td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
    <tr><td>UNDELIV_702</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_815</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_771</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_711</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_627</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_814</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_660</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_612</td><td>电信</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>UNDELIV_613</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_619</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_680</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_636</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_726</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_718</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_880</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_634</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_010</td><td>电信</td><td>短消息超过有效期</td><td>手机终端超时未响应</td></tr>
    <tr><td>EXPIRED_619</td><td>电信</td><td>短消息超过有效期</td><td>手机终端超时未响应</td></tr>
    <tr><td>EXPIRED_999</td><td>电信</td><td>短消息超过有效期</td><td>手机终端超时未响应</td></tr>
    <tr><td>UNDELIV_001</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>UNDELIV_620</td><td>电信</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>请核实手机终端是否处于正常状态</td></tr>
    <tr><td>EXPIRED_614</td><td>电信</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>EXPIRED_618</td><td>电信</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>EXPIRED_613</td><td>电信</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>EXPIRED_617</td><td>电信</td><td>运营商内部错误</td><td>无</td></tr>
    <tr><td>UNDELIV_701</td><td>电信</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>UNDELIV_701</td><td>电信</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>UNDELIV_802</td><td>电信</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>UNDELIV_801</td><td>电信</td><td>空号、停机或关机</td><td>无</td></tr>
    <tr><td>UNDELIV</td><td>电信/联通</td><td>用户因为状态不正确如处于停机、挂起等状态而导致用户无法接收到短信</td><td>无</td></tr>
    <tr><td>MOBILE BLACK</td><td>电信/联通</td><td>号码为全局黑名单</td><td>请联系<a href="/doc/product/382/3773">sms helper</a>解除黑名单</td></tr>
    <tr><td>其他</td><td>电信/联通</td><td>运营商未公布原因</td><td>请提供具体号码给<a href="/doc/product/382/3773">sms helper</a>，下工单向运营商核实</td></tr>
  </tbody>
</table>