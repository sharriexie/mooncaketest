资源|默认限制|最大限制
---|---|---
单个订阅中的 Azure 媒体服务 (AMS) 帐户数||25
每个 AMS 帐户的资产数||1,000,000<sup>1</sup>
每个作业的链接任务数||30
每个任务的资产数||50
每个作业的资产数||100
每个 AMS 帐户的作业数 ||50,000<sup>2</sup>
一次与一个资产关联的唯一定位符数||5<sup>4</sup>
每个 AMS 帐户的实时频道数 </p></td>|5</p></td>|N/A<sup>1</sup>
每个频道的停止状态节目数 </p></td>|50</p></td>|N/A<sup>1</sup>
每个频道的运行状态节目数 </p></td>|3</p></td>|3
每个 AMS 帐户处于运行状态的流式处理终结点数</p></td>|2</p></td>|不适用<sup>1</sup>
每个流式处理终结点的流式处理单位数 </p></td>|10 </p></td>|不适用<sup>1</sup>
每个 AMS 帐户的编码单位数 </p></td>|25</p></td>|不适用<sup>1</sup>
存储帐户 | |1,000<sup>5</sup>
策略 || 1,000,000<sup>6</sup>

<sup>1</sup> 你可以通过开具支持票证，来请求更新此配额的限制。不要通过创建更多 AMS 帐户来提高限制，而是应提交支持票证。

<sup>2</sup> 这个数字包括已排队的、已完成的、活动的和已取消的作业。不包括已删除的作业。可以使用 **IJob.Delete** 或 **DELETE** HTTP 请求删除旧作业。

<sup>3</sup> 发出列出作业实体的请求时，每个请求将最多返回 1,000 个实体。如果需要跟踪所有已提交的作业，可以使用 top/skip，如 [OData 系统查询选项](http://msdn.microsoft.com/zh-cn/library/gg309461.aspx)中所述。

<sup>4</sup> 定位符不用于管理按用户的访问控制。要为不同用户提供不同的访问权限，请使用数字权限管理 (DRM) 解决方案。

<sup>5</sup> 存储帐户必须来自同一 Azure 订阅。

<sup>6</sup> 不同的 AMS 策略限制为 1,000,000 个（例如，对于定位器策略或 ContentKeyAuthorizationPolicy）。如果经常使用相同的天数/访问权限等，则应使用相同的策略 ID。

<!---HONumber=Mooncake_0905_2016-->