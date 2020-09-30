# <Project Name>

Before submitting a PR containing your team's project information:
- Make sure you rename this file to contain your project's name
- Respond to add your response in each section below

## (0) Registration Submission, Project Name, and Team Slack Handles

*Please provide the Submission ID from your [Slingshot registration confirmation](https://slingshot.filecoin.io/register-now).  Also, confirm your project's name and the Filecoin Slack handles for your teammates.*
  project: 
	SingersMusic

	Slack: (url:https://app.slack.com/client/T01B4QHHR47/C01BRNGKN5A)
	gctechtalk.slack.com

## (1) Brief Project Description

*Add your project's description here.*
一款为自己打造的音乐网站,分为歌曲丶歌者两大类.让人人都可以拥有自己的音乐网站.
(A music website built for yourself, divided into two categories: songs and singers. Everyone can have their own music website.)

## (2) Link to Project UI

*Please include a link to your project application or UI. It does not need to be super polished or completely functional. We will be reviewing this link periodically to verify that your project is eligible for final rewards.*
下面是我们的链接:http://singersmusic.gctech.xin/请用尽量使用电脑浏览器打开
(Here is our link: http://singersmusic.gctech.xin/ Please use your computer browser to open)

## (3) What does your application/UI do?

*Give us a brief description of what your application/UI does and how users are intended to interact with it.*
通过登录注册账号,创建一个属于自己的音乐网站.你可以把自己喜欢的音乐下载下来,或者喜欢的歌星添加进去,上传后不会担心歌曲下架,一个属于自己的小天地.
(Create your own music website by logging in and registering your account. You can download your favorite music or add your favorite singers to it. After uploading, you won't worry about the song being off the shelves, a small world of your own.)

## (4) If your project is using a curated dataset, which one are you using?

*You can reference the [list of curated datasets in this repo](https://github.com/filecoin-project/slingshot/blob/master/datasets.md). If you'd like to use a dataset that is not on that list, please nominate your chosen dataset by updating the curated datasets table in this PR. If nominating a dataset, do you own or have exclusive rights to the data you plan to use?*
暂且未使用官网数据,数据来源用户.未来会使用
(The official website data has not been used for the time being, and the data comes from users. Will use it in the future)

## (5) If your project is not using a curated dataset, please tell us a little bit more about your data by answering the questions below.

*What sorts of data will you collect? Do you own or have exclusive rights to the data you plan to use? Is the data license available online? Does the data contain any sensitive or illegal information?*
数据来源用户
(Data source user)

## (6) How much data are you planning to store to the Filecoin network during the Slingshot competition?

*Give us as realistic an estimate as you possibly can at this stage. We understand it's impossible to have perfect information before really starting your project!*
大概1t(正式参与比赛只会更多)
About 1t (Official participation in the game will only be more)

## (7) How are you structuring the data?

*Is this structured or unstructured data? What data formats, schemas, etc. does this dataset follow?*
非结构化数据，这些数据可以是文本文件、图片、音视频等。 
(Unstructured data, these data can be text files, pictures, audio and video, etc.)

## (8) What pre-processing are you doing before ingesting the data?

*How will you prepare this data for ingestion into Filecoin? What size storage deals will you be making? If this is a tabular dataset or directory structure, how will you maintain indices into the data so you can retrieve specific data as needed for your application? This is currently one of the most important steps to being successful with data storage on Filecoin. Feel free to ask for help and/or look at docs for recommendations!*

我们会先将数据上传到IPFS中，然后通过IPFS导入到filecoin中。我们使用mysql来维护目录索引。 
(We will upload the data to IPFS first, and then import it into filecoin through IPFS. We use mysql to maintain the catalog index.)
## (9)  What tech stack will you use to store the data?

*Either: Powergate, Hosted Powergate, Textile Hub/Buckets, lotus, or some other solution. Tell us what you're planning to use and how.*

## (10) How will you retrieve the data?

*Share some more information about the data retrieval plans for your application? How often does the data need to be retrieved? What is the size of each individual read? Do you need to retrieve from Filecoin (colder storage) or from an intermediate caching layer, like IPFS? How will your application/UI retrieve the necessary data and expose it/interact with it in the UI?*
首先我们会将数据存储到IPFS中，将IPFS中文件的CID保存到Mysql数据库中，然后将IPFS中的数据导入到Filecoin上，当矿工成功达成存储交易后，我们会将Filecoin的CID也保存到Mysql中。IPFS从中起到了写入缓存的作用，同时还作为热数据缓存。 (First, we will store the data in IPFS, save the CID of the file in IPFS to the Mysql database, and then import the data in IPFS to Filecoin. When the miner successfully completes the storage transaction, we will also save the CID of Filecoin to Mysql. IPFS serves as a write cache from it and also serves as a hot data cache.)

## (11) Who is the intended user for your application/UI?

*Who do you anticipate will use your project/dataset?*
青少年,偏向于爱音乐的人 (Teenagers, who prefer music)

## (12) Do you have any users already or plans to acquire users soon?

*Yes/no. Also, please tell us a little bit about your future plans for user acquisition.*
1.网站线上线下的推广   (Online and offline promotion)
2.策划活动  (To plan an event)

## (13) What challenges do you anticipate with this project?

*We'd love to know what you're most worried about so we can help as much as possible. Let us know what you anticipate to be the biggest challenges with this project!*
担心用户存储过多,担心资料会过期问题,提供更多的音乐相关资料 (Worried about the user's excessive storage, worried that the data will expire, and provide more music-related data)
