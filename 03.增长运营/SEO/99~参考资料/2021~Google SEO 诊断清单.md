> [原文地址](https://www.zhidaow.com/post/google-seo-checklist-2021)

# Google SEO 诊断清单

# 1. 平台注册

平台注册主要是方便了解网站流量数据、SEO 各项数据，方便后续 SEO 的各种操作，主要推荐 GSC、GA 统计、Bing Webmaster Tools、Google Tag Manager 这 4 个平台的注册，是基础中的基础。

## GSC 是否注册

GSC，全称是 Google Search Console，是 Google 官方的站长工具，是 Google SEO 必备的一个平台。

主要有以下几个功能：

- Google 官方的数据反馈，如 Google 官方的流量、关键词、网页、索引等数据；
- 数据的提交和操作。如 sitemap、内容删除；
- 了解官方的问题反馈。比如网页未收录的问题、性能的问题、结构化数据的问题等，方便发现并解决问题。

下图是我博客的 GSC 截图：![img](https://www.zhidaow.com/SEO%20/_image/1.%20gsc.png?w=600)

地址：https://search.google.com/search-console （需翻墙）

## GA 统计是否安装

GA 统计是 Google 推出的免费的网站统计和分析工具，不光是流量统计功能，还有用户访问情况、转化情况等，是每个网站不可缺少的。
如果国内用户也可以用百度统计、CNZZ 等其他流量统计工具。
如果有做 Google ads，那 GA 统计就更有必要安装了。

## Bing Webmaster Tools 是否注册

如果做英文 SEO，最好也注册下 Bing Webmaster Tools，毕竟 Bing 仍是全球第二大搜索引擎。而且运营成本不高，只需要提交下 sitemap（格式通用），而且偶尔看下有没有异常的数据情况。

> 地址：https://www.bing.com/webmasters/

## Google Tag Manager 是否安装

GTM 是 Google 推出的网站代码片段管理工具，可以直接在后台进行网页代码的编辑和上线，非常简单便捷。不过可能网站具备较多改动需求、一定的技术能力才会用到。前期可以先不注册。

> 地址：https://marketingplatform.google.com/about/tag-manager/ （需翻墙）

# 2. 基础检查

主要是检查网站整体的基础配置情况，包含 robots.txt 和 sitemap 的检查。

## robots.txt 正确配置

robots.txt 主要是屏蔽搜索引擎爬虫对特定网页的抓取和索引，robots.txt 主要有两方面检查 ：

- 检查重要网页是否被 robots.txt 屏蔽，比如产品页、资讯页等
- 添加屏蔽规则，使某些网页屏蔽抓取，比如涉及用户隐私的频道等

- 参考文档：

  - 《创建 robots.txt 文件》：https://developers.google.com/search/docs/advanced/robots/create-robots-txt?hl=zh-cn
  - robots.txt 测试工具：https://www.google.com/webmasters/tools/robots-testing-tool?hl=zh-CN （需验证 GSC）

## sitemap 提交且可抓取

检查 GSC 和其他站长工具中是否有提交 sitemap，以及 sitemap 是否正常提交。下图中 sitemap 就出现了问题，导致无法正常提交网页。

![已提交的站点地图](https://www.zhidaow.com/SEO%20/_image/2.%20sitemap.png?w=600)

另外，sitemap 还需要注意的是：

- 不光是网页可以生成并提交 sitemap，视频、图片、新闻也需要提交 sitemap
- sitemap 可以帮助 Google 发现新网页，建议所有网站都生成和提交，尤其是大型网站、新网站
- sitemap 支持 xml、RSS、mRSS 和 Atom 1.0，以及 txt 格式
- 目前 Google 会忽略掉 sitemap 中 `<priority>` 和 `<changefreq>` 值（又一个以前关注的 SEO 小细节消失了）
- sitemap 不光可以在 GSC 提交，还可以通过 ping 工具、robots.txt 的方式提交

另外还有个小技巧，对于 Google SEO，建议每个目录提交一个 sitemap 文件。这样可以根据 sitemap 的数据报告得出每个目录的收录情况（Google 没有提供目录的收录数据）。

> 《创建和提交站点地图》https://developers.google.com/search/docs/advanced/sitemaps/build-sitemap?hl=zh-cn

# 3. 站内 SEO

站内 SEO 部分主要是使网站符合 SEO 的基本规范，并且能达到可抓取、可索引和排名的阶段。分为 URL、Title、Description、图片优化、视频优化、结构化数据等部分。

## URL 是否唯一、简单可读

URL 要做到 2 点：唯一、简短和可读性。唯一性是保证网页可收录，因为网页的 URL 是抓取、索引和排名的唯一标识，需要做到一个网页对应一个 URL，而避免出现一个网页有多个版本的 URL，导致自身重复，权重分散，常见的情况有带参数和不带参数，域名的规范配置，比如：

- `https://www.zhidaow.com/post/about` - 正常的规范 URL
- `https://www.zhidaow.com/post/about?rel=sayhi` - 加了参数导致 URL 不唯一
- `https://zh.zhidaow.com/post/about` - 又用了另外的 zh 二级域名出现了 URL 不唯一

另外，简短和可读性是直接影响用户点击，比如下面两个 URL：

- `https://www.zhidaow.com/post/google-seo-checklist-2021` - 简短可读，用户点击意愿强
- `http://www.example.com/index.php?id_sezione=360&sid=3a5ebc944f41daa6f849f730f1` - URL 较长，且看起来比较无意义，点击时会有犹豫

URL 、Title 和 Description 都是直接展示在 Google SERP 中，会直接影响点击率和流量。如下图：

![Google 搜索提示](https://www.zhidaow.com/SEO%20/_image/3.%20serp.png?w=600)

> 《保持简单的网址结构》https://developers.google.com/search/docs/advanced/guidelines/url-structure?hl=zh-cn

## Title 是否正确填写

Title 是网页中的 `<title>` 字段设置，会直接影响 Google 对网页主题的理解，以及网页在 SERP 中的展示。Title 检查时一般要注意几点：

- 每个网页都有单独的 `<title>`。很多企业站是全站 Title 都用同样的内容，无法正常表现每个网页的主题
- Title 要简单描述网页主题，比如某个的产品页 Title：`儿童极简护眼 LED 台灯，白色，流线型，触摸开关，三档调节`
- Title 要包含用户热搜词，这样能更好的命中用户需求，而且在 SERP 中也会有“飘红”展示，容易被用户点击，增加点击率（虽然 Google 的语义理解增强，同义词或模糊匹配也能有排名，但还是尽量完整出现）
- Title 中最好展示产品品牌、网站品牌。产品品牌可以增加用户关注，网站品牌则可以增加自身品牌曝光，比如 `儿童极简护眼 LED 台灯，白色，流线型，触摸开关，三档调节 - 你懂我台灯网`
- Title 中避免关键词重复和堆砌。早期可能有用，但现在并不建议，因为关键词重复和堆砌会影响可读性，而且现在已经失效了。

另外还要注意，站长设置的 Title 字段不一定会被 Google 采纳。Google 有时候会改写网页的 Title，比如根据用户的搜索次进行改写，或者算法给出更有描述性的标题。不过这个是正常情况，无需担心。

> 《在搜索结果中显示良好的标题和摘要》https://developers.google.com/search/docs/advanced/appearance/good-titles-snippets

## Description 是否正确填写

Description 是网页中的 `<meta name="description">` 字段，主要是网页内容的简述，像上图也会展示 Google SERP 中。Description 检查时也有几个注意要素：

- 每个网页都要有单独的 Description
- Description 要简述网页内容。比如文章页的 Description 可以是内容的摘要，产品页的 Description 可以是产品的核心属性，用户在浏览时能很方便了解到大概信息，更容易点击，例如：`淘宝为您提供儿童极简护眼 LED 台灯；颜色：白色；品牌：淘宝心选；光源类型：LED；开关类型：触摸开关；电压：111V~240V；价格：139.00元；邮费：包邮。`

对于一些大规模的网页，Description 和 Title 虽然只能采用模版的方式，但建议尽可能多的使用多个属性，这样让所有网页的 Description 更有描述性，也会更好匹配用户的搜索词。

另外，keywords 字段已经被 Google 忽略了，没有任何意义。所以一般情况下 keywords 可以不设置，或者跟 Title 一致。

> 《在搜索结果中显示良好的标题和摘要》https://developers.google.com/search/docs/advanced/appearance/good-titles-snippets

## 图片是否提交和优化

很多朋友认为图片只是 SEO 中的一项优化元素，其实图片的流量价值很高，之前在 alibaba 和 aliexpress 每天都有较大规模的流量来自图片。而且 Google 现在图片搜索中也加入了产品的标签以及库存信息，方便用户在图片搜索时直接浏览和转化。所以，图片优化可以跟网页优化同一等级来看。下图红框部分带有 Product 标志的是电商产品。

![](https://www.zhidaow.com/SEO%20/_image/3.%20image.png?w=600)

图片需要做一些优化，方便搜索引擎更好的理解和收录，也方便用户浏览。图片的 SEO 检查有几个方面：

- 图片内容检查。图片是否添加 alt 标签（具有描述性，避免堆砌）；图片名称中是否嵌入关键词（如 my-little-cat.jpg）；图片周围是否有一些描述文字
- 图片性能检查。图片最好使用 WebP 等性能更佳的格式；图片尺寸最好跟展示尺寸匹配，避免图片过大浪费性能；图片最好采用自适应图片
- 图片提交检查。是否使用结构化数据、sitemap 提交图片，提升图片的索引效率。

> 《Google 图片最佳做法》https://developers.google.com/search/docs/advanced/guidelines/google-images?hl=zh_cn
> 《图片站点地图》https://developers.google.com/search/docs/advanced/sitemaps/image-sitemaps?hl=zh_cn

## 视频是否提交和优化

作为新的内容形态，视频比文本和图片更生动。Google 也支持了视频的抓取和索引，并且新开了 Video 类型的搜索。从实际测试来看，视频是有额外的流量增量。所以，建议针对视频进行提交和优化。视频主要检查几个方面：

- 视频是否提交 sitemap 和结构化数据
- 视频内容和缩略图是否能被 Googlebot 抓取，而不是屏蔽状态
- 视频也可以放在 YouTube 等平台，然后在网站中嵌入使用
- 视频还可以使用视频预览和重要时刻的功能

![视频优化](https://www.zhidaow.com/SEO%20/_image/video%20case.png)

> 《视频最佳做法》https://developers.google.com/search/docs/advanced/guidelines/video?hl=zh_cn
> 《视频 Sitemap 及其替代方案》https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?hl=zh_cn

## 结构化数据是否配置

结构化数据是向 Google 提交一些支持的结构化数据，方便 Google 更好的理解和收录内容，并且在 SERP 会有特殊展示。结构化数据可以非常直观的提升 SERP 结果，对点击率和流量有明显提升。因此是非常建议选择合适的结构数据并添加在网页中的。以下是结构化数据的几种展现形式：

![结构化数据](https://www.zhidaow.com/SEO%20/_image/3.%20structured-data.png?w=600)

另外，比较常用的会有：

- Article
- Product
- 面包屑导航
- Logo
- 评价摘要
- Video

这里需要检查网站是否添加了结构化数据，并且是否完整、准确。另外，在 GSC 里也能看到结构化数据的收录数据，以及是否有字段问题。

> 《结构化数据常规指南》https://developers.google.com/search/docs/advanced/structured-data/sd-policies?hl=zh_cn

## 内部链接是否引导用户和爬虫访问

以前很多 SEO 会用内链来提升关键词的排名，但现在 Google 已经基本不用内链来传导权重，更多的是帮助 googlebot 发现新网页，帮助抓取。内链有 3 个检查项目：

- 网站是否使用链接建立了合理的架构，频道的上下级和相互间是否用内链很自然的串联起来；
- 内部链接的锚文本是否具有描述性，帮助搜索引擎理解下个页面的内容，以及引导用户点击；
- 网站的导航、面包屑导航是否正常使用链接。

下图是根据内部链接建立的简单的网站架构示例：

![页面面包屑导航](https://www.zhidaow.com/SEO%20/_image/3.%20website%20structurs.png?w=500)

下图的 toppage、News、Product list 都用 baseball card 这个锚文本指向某个产品页面，帮助用户和搜索引擎了解了这个页面的内容。

![面包屑导航](https://www.zhidaow.com/SEO%20/_image/3.%20inner%20links.png?w=500)

> 《搜索引擎优化 (SEO) 新手指南》https://developers.google.com/search/docs/beginner/seo-starter-guide?hl=zh_cn

# 4. 关键词研究

有些网站仅从卖方视角展示自己的能力和产品，其实也需要有买方视角：了解目标用户在搜索场景的需求，用哪些关键词在找产品，有什么样的搜索习惯，这样才能更好的匹配用户需求。这里就需要做行业的关键词研究。以下从整站关键词部署、关键词的选用和覆盖、关键词排名的策略和节奏、行业关键词库来检查。

## 整站关键词是否正确部署

检查整站的关键词部署情况，每个频道是否“各司其职”，有对应的关键词部署。这是从网页出发找到匹配的关键词部署的思路。如下图：

- 首页一般部署公司名称和行业大词，比如 “南京你懂我灯具公司 - 中国知名儿童台灯生产企业”
- 列表页部署产品名称关键词（热度中等），比如 “儿童护眼台灯 - 你懂我灯具”
- 文章页则部署具体的产品名称（偏长尾），如“儿童极简护眼 LED 台灯，白色，流线型，触摸开关，三档调节 - 你懂我台灯网”
- 资讯详情页部署内容型关键词，比如“儿童护眼灯怎么选”、“买儿童护眼灯应该注意哪些问题”等。

![关键词](https://www.zhidaow.com/SEO%20/_image/4.%20all%20words.png?w=400)

## 关键词是否正确选用，以及覆盖情况

如果各频道的关键词配置好了，就需要检查下这些关键词选用的是否合适，以及覆盖度情况。关键词怎么算合适呢？有以下几个方面：

- 是否有搜索量。这个词是否有用户搜索，每个月是否有一定的搜索量，而不是自己臆想出来的。
- 是否精准、有转化。这个词是否跟页面内容匹配，是否能通过这个词找到目标用户。

对于关键词的覆盖，这个需要有更全局的视角，能掌握行业的关键词和用户需求，然后来判断网站目前的关键词覆盖，还有多少的空间，之后往哪个方向去扩充。

## 关键词排名是否有合适的策略和节奏

网站需要根据自身情况来制定关键词策略，比如新站需要瞄准竞争度较小的内容关键词和产品关键词，而有一定权重的网站则需要做中等热度的关键词。这个需要了解网站情况才能判断，一般来说有以下的节奏：

- 新站建议先做搜索量小，竞争度小的内容关键词、产品关键词，例如内容和产品详情页，以及公司名称
- 中等权重的网站建议尝试做一些搜索量和竞争度中等的关键词，以及一些转化高，精准的关键词
- 高权重网站建议做搜索量更高、转化率更高的关键词，比如“南京二手房”，“南京旅游攻略”

## 行业关键词库的整理情况

如果真的要把某个行业做深吃透，是需要有个行业关键词库。虽然不一定非要把每个词都整理出来，但至少搜索量高的词是哪些，大多数用户的搜索需求在哪里，这个是要有数的。有了行业词库和需求的整体认知，你会知道网站的需求覆盖程度，之后怎么扩展；

也可以抽象出关键词 pattern，从而自己匹配出更多关键词；也可以根据用户需求来优化页面内容，在满足用户主要需求的同时，也能满足次要需求。所以，这个需要投入一些精力和研究才能了解，下图是一个简单的词库示例。

![行业词库](https://www.zhidaow.com/SEO%20/_image/4.%20keywords%20lab.png)

# 5. 技术 SEO

## 网站稳定性

主要检查网站能否保证用户正常访问、保证爬虫正常抓取，以及长期的稳定情况。

- 这里的用户是目标用户，而不是站长自己。比如国内有些英文独立站把服务器放在国内，每次自己访问的时候挺正常，殊不知国外的目标用户访问时需要等待较长时间；
- 容易被忽略是爬虫的抓取。Google 的大多数爬虫服务器是在美国，所以需要兼顾到 googlebot 在美国地区的抓取。
- 另外，网站经常宕机，出现 5xx，404 的返回码，也会影响网站的流量。

## 网站是否可抓取和收录

检查网站是否能够被正常抓取和收录，这里不光要检查 robots.txt 文件，还需要用 GSC 的网址检查工具，测试 Googlebot 的真实访问情况。有时候服务器端、HTTPS 头部也会影响爬虫抓取。下图是我博客某个网页的检查情况。还可以点击 “测试实际网址” 进行实时测试。

![Google Search Console](https://www.zhidaow.com/SEO%20/_image/5.%20check%20crawl.png)

下图是未收录时的各项信息，方便进一步的排查问题。

![覆盖率](https://www.zhidaow.com/SEO%20/_image/4.%20crawl%20error.png)

> 《Googlebot》https://developers.google.com/search/docs/advanced/crawling/googlebot
> 《索引简介》https://developers.google.com/search/docs/beginner/intro-indexing?hl=zh_cn

## 网站是否使用 HTTPS

HTTPS 协议是比 HTTP 更安全的一种协议，目前已经加入 Google 的排名因素中。检查网站是否全站使用 HTTPS 协议。如果网站没有用 HTTPS 协议，在排名上就会稍稍落后，所以最好配置上。

> 《使用 HTTPS 确保网站安全》https://developers.google.com/search/docs/advanced/security/https?hl=zh_cn

## 性能是否存在优化空间

性能优化也是 Google 排名因素之一，而且也直接影响用户的转化。可以重点做两项检查：

- 通过性能检测工具，测试核心网页的性能情况，是否有性能提升的机会点
- 通过 GSC 了解整站的 CWV 指标情况，CWV 优化是否有机会点（CWV 是 核心网页指标，之前我有[专门解读](https://www.zhidaow.com/post/google-core-web-vitals)）

这里推荐两个性能测试工具：

- gtmetrix.com
- webpagetest.org

这两个工具能对常见的性能指标和 CWV 指标进行测试。下图是对 alibaba 某个页面的检测：

![gtmetrix](https://www.zhidaow.com/SEO%20/_image/4.%20pagetest.png)

![webpagetest](https://www.zhidaow.com/SEO%20/_image/4.%20pagetest.png)

> 《了解 Google 搜索结果中的网页体验》https://developers.google.com/search/docs/advanced/experience/page-experience?hl=zh_cn

## 移动友好性情况

在移动时代的今天，移动端流量的重要性就不用多少，根据 GlobalStats 统计，手机端流量已经占到 55.77%。

![移动友好性](https://www.zhidaow.com/SEO%20/_image/5.%20mobile%20.png)

这里主要检查三点：

- 网站是否支持移动端访问
- 网站是否有做好移动端适配的配置：Google 支持自适应、动态提供内容、单独网址这 3 种移动配置
- 网站是否转为移动索引优先，网站主题内容是否两端一致，如果已经是移动索引优先，需要避免移动端流量的丢失

如果移动端未配置成功，至少损失一半流量。

> 《选择移动版网站配置 》https://developers.google.com/search/mobile-sites/mobile-seo?hl=zh_cn
> 《关于“优先将移动版网站编入索引”的最佳做法》https://developers.google.com/search/mobile-sites/mobile-first-indexing?hl=zh_cn

## JavaScript SEO 检查

早期 SEOer 会 “闻 JavaScript 色变”，认为 JavaScript 是对 SEO 不友好的。但 Google 现在已经可以解析 JavaScript 的内容了。 JavaScript SEO 主要检查几个方面：

- JavaScript 内容是否可被 googlebot 识别：可以通过 GSC 的实时测试，看 Googlebot 是否能识别到 JavaScript 内容
- 链接是否对 SEO 友好：链接的 `href` 值需要是正常链接，而不是 JavaScript 链接
- 列表页懒加载的方式是否对 googlebot 友好
- JavaScript 是否影响页面性能
- AJAX 部分是否可抓取和收录

上图是 Googlebot 目前的标准流程，已经加入了 JavaScript 的渲染，可识别 JavaScript 的内容：![img](https://www.zhidaow.com/SEO%20/_image/5.%20googlebot-crawl-render-index.png)

> 《JavaScript SEO 完全指南【2021 版】》https://www.zhidaow.com/post/javascript-seo-2021
> 《了解 JavaScript SEO 基础知识》https://developers.google.com/search/docs/guides/javascript-seo-basics
> 《实现动态呈现》https://developers.google.com/search/docs/guides/dynamic-rendering

## 死链情况是否正常

检查网站内存在的 404 网页情况，是否有正常网页提示 404 或软 404 的情况。通常检查的方法有：

- GSC - 索引率 - 已排除的 404 和软 404
- 服务器 log 中 googlebot 抓取的 404
- 用 screaming frog 抓取自己网站，发现站内的 404 网页

需要注意的是，爬虫抓取数据中存在一定数量的 404 是正常的，因为网站日常也有删除网页，产品下架的情况。这里主要是判断正常网页是否存在访问问题，出现 404 。

> 《“索引涵盖范围”报告》https://support.google.com/webmasters/answer/7440203?hl=zh-Hans#not_found_404

## 内容优化

内容方面，主要是检查网站内容是否能满足用户需求、是否有顺畅的阅读体验、E-A-T 情况、转化引导，以及网站本身在互联网是否有存在价值等。

## 需求满足程度

网页内容最基本的存在价值就是能满足用户的需求，而网页有特定主题（对应有关键词），就需要满足背后的主要需求，最好也能满足其次要需求。比如 “儿童护眼台灯怎么挑选” 这个主题（关键词），内容一定要能帮用户解答这个问题，给出一些挑选护眼台灯的建议，比如要 LED 光源，有亮度调节功能等。

再优质的内容，可以按照价格区间（如 200 以内、200 ～ 500、500 以上）、年龄段（如 3 ～ 5 岁、5 ～ 10 岁、10 岁以上）、不同品牌（如飞利浦、小米、华为等）；并推荐具体的几款产品和型号，最好再加上购买链接。如果要满足次要需求，可以再给用户推荐 “儿童护眼台灯评测 2021 版”、“儿童护眼台灯品牌排行前十名”，以及 “儿童书桌怎么挑选”、“儿童应怎么养成护眼习惯”等内容。

所以，内容检查时，基础要求是网页内容能满足用户的主要需求，更高要求则是是否有推荐内容，能满足次要需求。

## 阅读体验是否顺畅

阅读体验是指是否使用一些小技巧，增强内容的可读性，对用户和 SEO 都有帮助。主要有以下几个小技巧：

- 内容是否使用小标题
- 内容是否加图片、视频
- 内容是否有用短句和短段落
- 是否有合适的内链引导用户浏览
- 是否有语法错误、拼写错误

## E-A-T 情况

Google 越来越关注网页的 E-A-T ，也就是网页内容的专业度、权威度和信任度。比如产品详情页，在专业度方面能否展示更多专业的数据、图表等；在权威度上能否展示作者的简介，行业资历；在信任度上，能否加上行业的资质证书、合作厂商等。下图是 CoSchedule 对 E-A-T 的简单解读。

![CoSchedule](https://www.zhidaow.com/SEO%20/_image/6.%20google-eat-algorithm-update.png)

> 《What is E‑A-T? Why It’s Important for SEO》https://ahrefs.com/blog/eat-seo/
> 《SEO 友好的电商产品页设计｜附 10+个实际案例》https://www.zhidaow.com/post/seo-friendly-ecommerce-product-pages

## 网页价值情况

我这里并没有说原创度，而是用网页价值。因为原创度并不是判断网页价值的唯一标准，主要是看网页是否有增益。而网页能否被搜索引擎收录，主要是判断网页价值。

比如内容增益，就是在原内容上增加相关信息，像新闻详情页，如果把这个新闻的相关背景加上，或者补充另外一个专家的看法，也是比原网页更有价值。

再比如站点增益，同样的新闻如果转载到新浪新闻，对用户有更多的权威度、信任度和稳定性，即便是重复也有价值（但仍推荐做内容增益）。如果大多数内容都是直接转载，也没有其他方面的增益，那网页价值就没那么高，从而影响收录情况。

> 《浅谈互联网页面价值》https://www.chinaz.com/web/2011/0608/186736.shtml

## 是否有做转化引导

每个网站都有终极目标，比如电商站就是为了用户下单和转化，社交媒体是希望用户关注和传播，一些内容站是为了用户订阅，或点击广告。所以，网站一定要添加清晰、醒目的行动号召元素，这样才能使流量价值最大化。比如电商站的首屏一定要有明确的下单按钮，独立站要有留言和询盘按钮，而内容页也需要有订阅和关注功能。

下图是 B 站对用户分享和关注的引导。

![转化引导](https://www.zhidaow.com/SEO%20/_image/6.%20cvr.png)

## 是否有外链增长机会点

外链，相当于其他网站在茫茫互联网中的投票，对排名有帮助作用。可以从以下 4 个方面检查外链是否有增长空间：

- 是否有可用的外链资源，比如朋友、同行网站是否能交换链接
- 一些丢失的外链是否能修复，比如通过 ahrefs.com 找出 404 外链并修复
- 网站是否有社交平台转发的功能
- 问答、社区、博客等平台是否能以交流和分享的方式来增加外链，比如 quora, reddit 等
- 能否跟进竞手的外链进行外链增长

另外，我不推荐外链购买等非白帽的方式，是违反 Google 指南，长期来看具有一定风险的行为。
