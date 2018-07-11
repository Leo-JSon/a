<template>
  <div class="container">
    <img src="../../assets/images/call.png">
    <div class="content-wrap">
      <Row>
      <Col span="4">
      <div class="leftmenu">
        <ul class="nav">
          <li class="divider">{{$t('cms.about')}}</li>
          <li><router-link to="/about-us">{{$t('cms.aboutus')}}</router-link></li>
          <li class="cur"><router-link to="/join-us">{{$t('cms.joinus')}}</router-link></li>
        </ul>
      </div>
      </Col>
      <Col span="20">
      <div class="content">

        <div class=WordSection1 style='layout-grid:15.6pt'>
            <pre style="white-space: pre-wrap;">
If you are strongly interested in Block chain industry
If you have a profound cognition in crypto currency
If you are armed with strong learning ability and, have great enthusiasm for work
Then, welcome to join DBEX! 

<b>Senior Product Manager</b> 

Job Responsibilities:
1. Responsible for the development planning and core module designing of the company's digital assets trading products;
2. Design and utilize data recovery mechanism to guide product optimization and perform iterative monitoring;
3. Responsible for the collection and in-depth analysis of competitive products, industry products, and industry-related information;
4. Analyze and measure the product life cycle, then giving constructive opinions on the long-term development strategy of the product. Providing reference for the company's decision-making.

Job requirements:
1. Strongly interested in the Internet financial industry and block chain technology, and a profound cognition of user groups that are being targeted;
2. Logic of the overall implementation process of Internet products should be clear. Can control the progress and quality of the project well, and coordinate the relevant personnel to complete tasks.
3. Have a keen market insight and have the abilities of logic analysis with good communication and collaboration skills. Also a solid technical understanding is needed;
4. Have a strong sense of goal orientation and execution, can lead the team to goal achievement with high efficiency;
5. At least 3 years in Internet products, with excellent interaction design skills, pursuit of the ultimate in user experience. Industry-related product experience is preferred.


<b>Senior/Advanced Mobile Product Manager</b>

Job Responsibilities:
1. Responsible for the development planning and core module designing of the company's mobile digital assets trading products;
2. Design and utilize data recovery mechanism to guide product optimization and perform iterative monitoring;
3. Responsible for the collection and in-depth analysis of competitive products, industry products, and industry-related information;
4. Analyze and measure the product life cycle, then giving constructive opinions on the long-term development strategy of the product. Providing reference for the company's decision-making.


Job requirements:
1. Strongly interested in the Internet financial industry and block chain technology, and a profound cognition of user groups that are being targeted;
2. Logic of the overall implementation process of Internet products should be clear. Can control the progress and quality of the project well, and coordinate the relevant personnel to complete tasks.
3. Have a keen market insight and have the abilities of logic analysis with good communication and collaboration skills. Also a solid technical understanding is needed;
4. Have a strong sense of goal orientation and execution, can lead the team to goal achievement with high efficiency;
5. At least 5 years in Internet products, with excellent interaction design skills, pursuit of the ultimate in user experience. Industry-related product experience is preferred. 



<b>Product assistant</b>

Job Responsibilities:
1. Responsible for the collection and analysis of competing products, industry products, and industry-related information;
2. Responsible for feedback and finishing related to product effects, and output usability effect suggestions;
3. Assist the department head to complete the routine work within the department.

Job Requirements:
1. Unified undergraduate education;
2. Priority students are preferred;
3. Interested in the Internet finance industry and block chain technology.


<b>Senior/Advanced UI Designer</b>

Job Responsibilities:
1. Responsible for the visual design of financial products, providing a global design;
2. Participate in product discussion, interaction design, promote technology restoration interface design, check and correct design problems, and be responsible for the final effect;
3. Participate in and formulate design principles and specifications to achieve a reconciled product visual style.

Job Requirements:
1. Graduated from design related majors and proficient in using relevant design tools;
2. Rich visual design experience for web pages and mobile products, and successful market cases are preferred;
3. Sensitive touch and comprehension of UI design trends;
4. Familiar with relevant interaction design and user research methods and workflows, able to independently support product design work;
5. Pay attention to details and pursue the ultimate experience;
6. Have a good cooperation attitude and team spirit, full of work passion. Creativity and responsibility.


<b>English Translator</b>

Job Responsibilities:
1. Responsible for the translation of daily English business;
2. Collection and translation of overseas industry market information;
3. English mail communication and translation.

Job Requirements:
1. Bachelor degree or above, text translation skills are profound;
2. Internet financial background is preferred;
3. Foreigners with Chinese-language basis, familiar with Chinese-English translation;
4. There are overseas study backgrounds, overseas life experiences, and overseas resources are preferred.


<b>Senior JAVA Development Engineer</b>

Job Responsibilities:
1. Research and development of the next generation bitcoin exchange and related systems;
2. Create performance indicators;
3. Rapid iteration based on feedback;
4. Working in a small team may involve different levels of development;

Job Requirements:
1. Skilled in using java;
2. Have many years of experience in actually writing code;
3. Understand basic relational database knowledge;

Optional skills:
Contribute to open source code or maintain a technical blog
Development experience with blockchain (bitcoin Ethereum)
Ability to develop and troubleshoot multi-threaded code
Experience with JVM development, configuration, tuning
Experience in optimizing existing programs
Ability to independently develop individual modules
Strong communication skills and ability to collaborate with cross-functional teams

 
<b>Workplace</b>

We are recruiting at the following locations with the following priorities: Dubai, Southeast Asia, then expanding to the world.

 
<b>Contact Us</b>

To apply for the above positions, please send your resume and cover letter to hr@mail.bcuae.com. Please indicate the desired position and place of work in the subject of the email.

            
              </pre>
        </div>

      </div>
      </Col>
      </Row>
    </div>
  </div>
</template>

<style scoped>
.postlist li {
  float: left;
  width: 50%;
}
li.header {
  width: 100%;
  text-align: center;
  font-size: 16px;
  padding: 10px;
  background: #ccc;
}
.postlist ul:after {
  content: " ";
  clear: both;
  display: block;
}
.container {
  /* background: #fff; */
  overflow-x: hidden;
}
.content-wrap {
  padding-top: 20px;
  position: relative;
  width: 1200px;
  margin: 20px auto;
  background: #222327;
}
.leftmenu {
  /*position: absolute;*/
  /*width: 180px;*/
  /*text-align: center;*/
  /* border: 1px solid #efefef; */
}
.leftmenu .divider {
  font-size: 20px;
  padding: 5px;
  color: #d58c2a;
  /* background: #efefef; */
}
.leftmenu li {
  font-size: 14px;
  line-height: 30px;
  padding: 5px;
}
.leftmenu li.cur {
  background: #323031;
  color: #b9ac9e;
}
.leftmenu li a {
  color: #9a9083;
}
.leftmenu li a:hover {
  color: #d58c2a;
}
.leftmenu li.cur a {
  /* color: #D58C2A ; */
}
.content {
  padding-top: 20px;
  /*padding-left: 200px;*/
  padding-bottom: 20px;
  text-align: left;
  padding-left: 20px;
}
.content p {
  text-indent: 2em;
  margin-bottom: 10px;
  font-size: 14px;
}
.content > div {
  padding-bottom: 20px;
}
.content h3 {
  font-size: 22px;
  font-weight: normal;
  margin-bottom: 20px;
}
.content h5 {
  font-size: 14px;
}
.WordSection1 pre {
  color: #665f57;
  font-family: 宋体;
  font-size: 16px;
  padding:0 40px;
}
</style>
