# X / Twitter 数据接口（X API）：帖子搜索、用户、关注、长串、社区、趋势

**X API · Twitter API · tweet search · Twitter followers · X trends**

这个仓库是 [DataXAPI](https://dataxapi.com/zh/?ref=gh-x-twitter-api) 的X（推特）接口说明和能直接跑的脚本：21 个接口，一把 Key，按次付费，$0.0001 起，**出错不收费**。不用登录平台账号，不用 Cookie，不开浏览器。

[免费拿 Key：试用最多 333 次，不用绑卡](https://dataxapi.com/zh/signin/?button=gh-x-twitter-api) · [全部接口文档](https://dataxapi.com/zh/apis/?ref=gh-x-twitter-api) · [接进 AI（MCP）](#接进-aimcp) · [English](#english)

最低充 $10，余额不过期；支持支付宝、微信支付和银行卡。

## 全部 21 个接口

### 社区

| 接口 | 拿到什么 | 价格 | 编号 |
|---|---|---|---|
| [X 社群帖子](https://dataxapi.com/zh/apis/x/communities/posts/list/) | 按社群编号取一页这个 X 社群里的帖子。 | 每条 $0.0003，一次最多 $0.006 | `x.communities.posts.list` |
| [X 社群资料](https://dataxapi.com/zh/apis/x/communities/get/) | 按社群编号取 X 社群的资料：名称、简介、成员数、管理员人数、加入方式、创建时间。 | $0.0004 一次 | `x.communities.get` |
| [X 社群成员](https://dataxapi.com/zh/apis/x/communities/members/list/) | 按社群编号取一页加入了这个 X 社群的账号，每页约 20 个：账号名、显示名、简介、粉丝数、是否认证。 | 每条 $0.0004，一次最多 $0.008 | `x.communities.members.list` |

### 列表

| 接口 | 拿到什么 | 价格 | 编号 |
|---|---|---|---|
| [X 列表帖子](https://dataxapi.com/zh/apis/x/lists/posts/list/) | 按列表编号取一页这个 X 列表时间线上的帖子，从最新的开始，每页约 100 条。 | $0.002 一次 | `x.lists.posts.list` |
| [X 列表关注者](https://dataxapi.com/zh/apis/x/lists/followers/list/) | 按列表编号取关注了这个 X 列表的账号，最多 20 个：账号名、显示名、简介、粉丝数、是否认证。只有这一页，不能往后翻。 | 每条 $0.0004，一次最多 $0.008 | `x.lists.followers.list` |
| [X 列表成员](https://dataxapi.com/zh/apis/x/lists/members/list/) | 按列表编号取一页这个 X 列表收录的账号，每页 20 个：账号名、显示名、简介、粉丝数、是否认证。 | 每条 $0.0004，一次最多 $0.008 | `x.lists.members.list` |

### 内容

| 接口 | 拿到什么 | 价格 | 编号 |
|---|---|---|---|
| [X 长文详情](https://dataxapi.com/zh/apis/x/posts/article/get/) | 按帖子编号取这条 X 帖子附带的长文：标题、全文、作者、发布时间、点赞、回复和浏览数。 | $0.002 一次 | `x.posts.article.get` |
| [X 帖子详情](https://dataxapi.com/zh/apis/x/posts/get/) | 按帖子编号或链接取一条 X 帖子：正文、作者、发布时间、点赞、回复、转推、引用、书签和浏览数。 | $0.0003 一次 | `x.posts.get` |
| [X 帖子引用列表](https://dataxapi.com/zh/apis/x/posts/quotes/list/) | 按帖子编号取一页引用它的 X 帖子，可按时间或按热门排。 | 每条 $0.0003，一次最多 $0.006 | `x.posts.quotes.list` |
| [X 帖子回复列表](https://dataxapi.com/zh/apis/x/posts/replies/list/) | 按帖子编号取一页这条 X 帖子下面的回复，按平台的相关度排；X 的回复本身是帖子，按帖子返回。 | $0.002 一次 | `x.posts.replies.list` |
| [X 帖子转推用户](https://dataxapi.com/zh/apis/x/posts/retweeters/list/) | 按帖子编号取一页转推了这条 X 帖子的账号：账号名、显示名、简介、粉丝数。 | $0.002 一次 | `x.posts.retweeters.list` |
| [X 帖子搜索](https://dataxapi.com/zh/apis/x/posts/search/) | 按搜索词找 X 帖子，可按热门或最新排；搜索词里可以用 X 自己的搜索语法，如 from:账号名。 | $0.002 一次 | `x.posts.search` |
| [X 视频字幕](https://dataxapi.com/zh/apis/x/posts/transcript/get/) | 按帖子编号或链接取 X 帖子里的视频说的话，全文；只支持两分钟以内的视频。 | $0.002 一次 | `x.posts.transcript.get` |

### 长串

| 接口 | 拿到什么 | 价格 | 编号 |
|---|---|---|---|
| [X 帖子对话串](https://dataxapi.com/zh/apis/x/threads/posts/list/) | 按对话串里任意一条帖子的编号，取这条对话串的帖子：主帖、作者的续帖和其中的回复。 | 每条 $0.0003，一次最多 $0.015 | `x.threads.posts.list` |

### 热榜和趋势

| 接口 | 拿到什么 | 价格 | 编号 |
|---|---|---|---|
| [X 趋势榜](https://dataxapi.com/zh/apis/x/trends/list/) | 取 X 当前的趋势榜前 30 条，带名次；可以取全球的，也可以取某个国家的。 | $0.009 一次 | `x.trends.list` |

### 账号

| 接口 | 拿到什么 | 价格 | 编号 |
|---|---|---|---|
| [X 用户粉丝列表](https://dataxapi.com/zh/apis/x/users/followers/list/) | 按账号名取一页关注该 X 用户的账号，每页最多 200 个，从最新关注的开始。 | 每条 $0.0001，一次最多 $0.02 | `x.users.followers.list` |
| [X 用户关注列表](https://dataxapi.com/zh/apis/x/users/following/list/) | 按账号名取一页该 X 用户关注的账号，每页最多 200 个。 | 每条 $0.0001，一次最多 $0.02 | `x.users.following.list` |
| [X 用户资料](https://dataxapi.com/zh/apis/x/users/get/) | 按账号名或编号取 X 用户资料：显示名、简介、粉丝数、关注数、是否有认证标和是哪种（企业金标、政府灰标）、自填的地点、网站；可一次传最多 100 个编号。 | 每条 $0.0004，一次最多 $0.04 | `x.users.get` |
| [X 用户提及](https://dataxapi.com/zh/apis/x/users/mentions/list/) | 按账号名取一页提及该 X 用户的帖子，从最新的开始。 | 每条 $0.0003，一次最多 $0.006 | `x.users.mentions.list` |
| [X 用户帖子列表](https://dataxapi.com/zh/apis/x/users/posts/list/) | 按账号名取一页该 X 用户主页上的帖子，从最新的开始；用 tab 选帖子、回复或媒体分栏。帖子分栏里有这个账号的转推，ext.is_retweet 标出来，并给原帖编号和原帖作者编号。 | $0.002 一次 | `x.users.posts.list` |
| [X 用户搜索](https://dataxapi.com/zh/apis/x/users/search/) | 按搜索词找 X 账号，每页约 20 个：账号名、显示名、简介、粉丝数、是否认证。 | 每条 $0.0004，一次最多 $0.008 | `x.users.search` |

## 真实返回长什么样

**X 帖子搜索**（`x.posts.search`，参数 `{"query":"weather forecast"}`），录下的真实返回，个人信息换成了 …：

```json
{
  "data": {
    "items": [
      {
        "id": "…",
        "url": "https://example.com/…",
        "type": "video",
        "text": "…",
        "lang": "en",
        "published_at": "2026-10-12T00:44:12.000Z",
        "author": {
          "id": "…",
          "username": "…",
          "name": "…",
          "avatar_url": "https://example.com/…",
          "verified": true,
          "followers": 7425
        },
        "metrics": {
          "likes": 238,
          "comments": 37,
          "favorites": 145,
          "views": 8357,
          "reposts": 121
        },
        "images": [],
        "hashtags": [],
        "mentions": [
          {
            "id": "…",
            "username": "…",
            "name": "…"
          }
        ],
        "post_id": null,
        "parent_id": null
      }
    ]
  },
  "page": {
    "next_cursor": "example-cursor-1",
    "cursor_expires_at": "2026-10-12T20:10:39.000Z",
    "has_more": true,
    "returned": 20
  }
}
```

每个接口都是同一种结构：列表在 `data.items`，单个在 `data.item`，下一页用 `page.next_cursor`，这次扣了多少在 `meta.billing.amount`，平台不给的字段为 `null` 并在 `meta.unavailable` 里写明。

## 快速开始

1. [拿一把 Key](https://dataxapi.com/zh/signin/?button=gh-x-twitter-api)（`dx_` 开头），放进环境变量：`export DATAXAPI_API_KEY=dx_...`
2. 调一次接口：

```bash
curl -G "https://api.dataxapi.com/v1/x/posts/search" \
  -H "Authorization: Bearer $DATAXAPI_API_KEY" \
  --data-urlencode 'query=weather forecast'
```

3. 或者跑 `examples/` 里的脚本。只用 Python 标准库（3.9 以上）；不加 `--yes` 只报价、不调用，加了才真跑，跑完告诉你实际花了多少：

| 脚本 | 做什么 | 先看要花多少 |
|---|---|---|
| [quickstart.py](examples/quickstart.py) | 取几页结果，存成 CSV | `cd examples && python3 quickstart.py 'weather forecast'` |

## 接进 AI（MCP）

Claude Code：

```bash
claude mcp add --transport http --scope user dataxapi https://api.dataxapi.com/mcp --header "Authorization: Bearer $DATAXAPI_API_KEY"
```

Cursor、Cherry Studio、WorkBuddy 等支持远程 MCP 的客户端：

```json
{
  "mcpServers": {
    "dataxapi": {
      "url": "https://api.dataxapi.com/mcp",
      "headers": {
        "Authorization": "Bearer dx_..."
      }
    }
  }
}
```

接上以后直接用中文问，比如“帮我看看这个关键词最近一个月在抖音上的热度”。AI 花钱前可以先免费查接口和价格。也可以装成技能：`npx skills add data-x-api/skills`。

## 常见问题

**要不要平台账号、Cookie 或扫码？**

不要。只要一把 DataXAPI Key，不碰你的账号，也就不存在账号被风控的问题。

**调用出错扣钱吗？**

不扣。每次返回里的 `meta.billing.amount` 写明这次扣了多少（美元）。

**数据有多新？**

默认在你调用时从平台实时读取，返回里的 `meta.fetched_at` 写明读取时间。

**怎么翻页？**

列表接口一次返回一页，把返回里的 `page.next_cursor` 作为 `cursor` 传回去取下一页，每一页单独计费。

## English

X (Twitter) API: post search with X search operators, users, followers, threads, communities, lists and trends, through one key, paid per call, no X developer account.

No platform account, cookie or QR login. Paid per call from $0.0001; errors are not charged. Free trial: up to 333 calls, no card. [Get a key](https://dataxapi.com/signin/?button=gh-x-twitter-api) · [All endpoints](https://dataxapi.com/apis/?ref=gh-x-twitter-api) · MCP: `https://api.dataxapi.com/mcp`.

## License

MIT

<sub>接口和价格取自 DataXAPI 的目录 720fc3ea8dadb865、价格版本 19；以 [dataxapi.com/zh/apis](https://dataxapi.com/zh/apis/?ref=gh-x-twitter-api) 为准。</sub>
