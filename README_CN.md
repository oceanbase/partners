# OceanBase 社区生态伙伴

[English](README.md)

OceanBase 社区生态伙伴是 [OceanBase 合作伙伴计划](https://www.oceanbase.com/partner)的一部分，按照伙伴的类型可以分为社区解决方案伙伴和社区产业生态伙伴。

## 社区解决方案伙伴

OceanBase 社区解决方案伙伴指的是所提供的与 OceanBase 社区版的联合解决方案通过了社区版兼容认证的生态伙伴。您可以访问我们的网站查看完整的伙伴列表 https://www.oceanbase.com/partner/solution 。

OceanBase 社区解决方案合作伙伴认证流程如下：

1. 填补[《测试报告模版》](solution/OceanBase数据库社区版&XXXX联合解决方案测试报告.docx)中的红色部分。
2. 在 [Who is using OceanBase](https://github.com/oceanbase/oceanbase/issues/1301) 中进行回复（中英文均可）。
3. 通过社区的[联系方式](https://github.com/oceanbase/oceanbase/blob/develop/README_CN.md#%E7%A4%BE%E5%8C%BA)联系相关工作人员，提交测试报告。
4. OceanBase 团队相关人员审核通过后，进行认证证书的电子签章流程。
5. 签章流程结束后，我们会给您认证证书，并将您更新到我们的网站。

## 社区产业生态伙伴

OceanBase 社区产业生态伙伴指的是 OceanBase 社区版在数据库业务内的生态伙伴，主要包括数据库工具、数据库中间件，以及芯片、操作系统等基础设施。

OceanBase 社区产业生态伙伴的信息目前全部存放在当前目录下，主要涉及以下几部分

- `partners.yml`: [产业生态伙伴列表](https://www.oceanbase.com/partner/product-ecology)中的社区生态伙伴信息，如您想对其进行更新，请直接创建一个修改本文件的 pull request。
- `landscape.yml`: [产业生态伙伴全景图](https://www.oceanbase.com/partner#ecology)中展示的社区产业生态伙伴列表，如您想对其进行更新，请先将其加入到 `partners.yml`，之后再创建 issue 进行申请，并在正文中附上对应的 400*128 像素的 logo 图片。
- `logo`: logo 图片存放目录，在您更新 landscape 的申请通过后，将由 OceanBase 团队的人员替您更新图片到该目录。

如需添加新合作伙伴，您需要提供以下信息：

```yaml
  - id: 必填，伙伴 id，由字母、数字和破折号组成，需要与伙伴名称一致。
    name: 必填，伙伴名称。
    website: 必填，伙伴的官网。
    description: 必填，伙伴的介绍。
    compatibility:
      - partner: 必填，伙伴产品的名称和版本。
        ob: 必填，OceanBase 的版本。
        category: 必填，伙伴产品的一级分类。
        subcategory: 必填，伙伴产品的二级分类。
    references:
      - title: 必填，链接的标题。
        url: 必填，链接的 url。
```

## 开源协议

本仓库中的产品信息和图标文件版权归属于创建它们的公司或组织，在此缓存只是为了提高展示网页的可靠性。仓库中的其他内容遵循 Apache 2.0 协议。
