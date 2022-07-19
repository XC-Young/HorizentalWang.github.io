如果您想对主页进行改动
- fork该项目到您个人账户;
- 将所fork的该项目下载到您本地进行修改;
- 提交您本地项目到您的账户;
- 在您的个人帐户项目中新建pull request等待拉取。

以下为修改指南：
- 如果您想添加Academic Activities，请在index.html的：
  ```
  <p class="lead" style="border-bottom:1px solid #CCC">Recent News</p>
	<ul>
	<li><font color="red"><b>I am looking for self-motivated students, postdocs, research assistants and visiting scholars! Please <a href="contact">drop me an email</a> if you are interested in working with me!</b></font></li>
  ```
  下方加入：
  ```
  <li>Your news</li>
  ```

- 如果您想将您的论文添加到主页：
  - 请准备：
    - 一张长宽比近似3：2的代表性图片(jpg/png/gif);
    - 文章标题;
    - 作者全名;
    - 所发表期刊/会议，奖项/分区/CCF级别
    - 相关网址链接（paper，code，project，slides，videos...）
  - 将图片加入到您复制到本地的文件夹/publications/teasers
  - 组织如下代码：
  ```
  	<div class="before-item" >
		<div class="pubimg">
			<img  class="pubpic" src="teasers/yourpic.jpg">
		</div>
		<div class="pubdsp">
			<span class=pubtitle > 
				Your Title<br>
			</span>
			<span class=pubauthor > 
				Authors, <b>Zhen Dong</b>, Authors<br>
			</span>
			<span class=publoc > 
				Your journal/reference (eg:CCF-A)<br>
			</span>
			<span class=publink>
				[<a href="Your paper link">Paper</a>]
				[<a href="Your code link">Code</a>]
				[<a href="Your video link">Video</a>]
			</span>
		</div>
	</div>
  ```
  - 确认年份及分类（Multi-modal Data Fusion/Point Cloud Augmentation/Scene Understanding/Scientistic Calculation/Reconstruction/Others）
  - 在 publication/index.html中查找
    ```
    <p class="lead" style="border-bottom:1px solid #CCC">Your year</p>
    ```
    在其下方加入您的上述文章代码
  - 在publication/index_topic.html中查找
    ```
    <p class="lead" style="border-bottom:1px solid #CCC">Your topic</p>
    ```
    在其下方加入您的上述文章代码
  -如果您的文章被选为selected展示
    在index.html中
    ```
    <p class="lead" style="border-bottom:1px solid #CCC">Selected Publications</p>
    ```
    下方加入您的上述文章代码

- 如果您想将您的项目添加到主页，请在projects/index.html的列表中加入
  ```
  <li>名字,时间段,主持。</li>
  ```

- 如果您想添加Awards，请在index.html的对应位置：
  ```
  <p class="lead" style="border-bottom:1px solid #CCC">Awards</p>
  ```
  下的列表中加入
  ```
  <li>名称(年份)</li>
  ```

- 如果您想添加Academic Activities，请在index.html的对应位置：
  ```
  <p class="lead" style="border-bottom:1px solid #CCC">Academic Activities</p>
  ```
  下的列表中加入
  ```
  <li>名称</li>
  ```