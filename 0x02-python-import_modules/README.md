## Alx software engeneer

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1">
<!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
<meta name="description" content="">
<meta name="google" content="notranslate">

<script>
window.dataLayer = window.dataLayer || [];
dataLayer.push({"userId":197885,"visitorType":"student","batch":{"id":26,"fullNameWithC":"AFR-1122 (C#11)","schoolLocation":{"id":1,"name":"ALX Africa"}},"curriculum":{"id":1,"name":"Foundations"}});

window.gtm_user_custom_event = function (name, options) {
if (typeof name === 'undefined') {
return;
}

window.dataLayer.push({
customEventOptions: typeof options !== 'undefined' ? options : {},
event: name,
});
}
</script>

<!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-N4C8MF2');</script>
<!-- End Google Tag Manager -->


<title>Project: 0x02. Python - import &amp; modules | ALX Africa Intranet</title>

<link rel="stylesheet" href="https://use.typekit.net/xgz4ilr.css">
<link rel="stylesheet" media="all" href="/assets/application_alx-1f48fe32f8890a5b4043ac403220430a9a865066a8afacdbbae3f3b7acb5e0c7.css" />
<script src="https://www.gstatic.com/charts/loader.js"></script>
<script src="/assets/application-28fbde0d9d7e01867b82fdb2a88556984777beb449e6fde74a7b722d6c9d640a.js"></script>
<link rel="shortcut icon" type="image/x-icon" href="/favicon_alx.ico" />
<meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="z9lU0DYAxbDH01y2BP1tvywgpYtbfebY4mHUoIv-29SSR8YDLYhsa2FDc6w-VDgv3VhLv5Abd-mgEKUHVZTkZw" />

<link rel="apple-touch-icon" href="/apple-touch-icon_alx.png">

<!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
<!--[if lt IE 9]>
<script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
<script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
<![endif]-->

<!-- Store user timezone -->
<script>
Cookies.set('timezone', (new Date()).getTimezoneOffset() / -60.0);
</script>

<!-- intro.js for interactive onboarding -->

<!-- React -->
<script src="/packs/js/application-74acb2dd7888fe19f18d.js"></script>
<link rel="stylesheet" media="screen" href="/packs/css/application-87456da7.css" />
</head>

<body class="signed_in env_production notranslate"
translate="no"
class="notranslate"
data-theme-suffix="_alx">
<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-N4C8MF2"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->


<input type="hidden" id="hbtn-slack-url" value="https://alx-students.slack.com">
<nav class="navbar navbar-default navbar-fixed-top topbar visible-xs">
<div class="navbar-header">
<button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar-mobile" aria-expanded="false">
<span class="sr-only">Toggle navigation</span>
<span class="icon-bar"></span>
<span class="icon-bar"></span>
<span class="icon-bar"></span>
</button>

<a class="navbar-brand" href="/">
<div class="logo"></div>
</a>  </div>

<div class="collapse navbar-collapse navigation" id="navbar-mobile">
<ul class="nav navbar-nav">



<li data-container="body" data-placement="right" data-toggle="tooltip" title="My Planning"><a href="/planning/me"><div class="icon "><i aria-hidden="true" class="fa fa-calendar "></i></div><div class="visible-xs">My Planning</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-current-projects-item" title="Projects"><a href="/projects/current"><div class="icon "><i aria-hidden="true" class="fa fa-code-fork "></i></div><div class="visible-xs">Projects</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" title="QA Reviews I can make"><a href="/corrections/to_review"><div class="icon "><i aria-hidden="true" class="fa fa-check "></i></div><div class="visible-xs">QA Reviews I can make</div></a></li>

<li data-container="body" data-placement="right" data-toggle="tooltip" title="Evaluation quizzes"><a href="/dashboards/my_current_evaluation_quizzes"><div class="icon "><i aria-hidden="true" class="fa fa-question "></i></div><div class="visible-xs">Evaluation quizzes</div></a></li>

<hr title="My resources">

<li data-container="body" data-placement="right" data-toggle="tooltip" title="Curriculums"><a href="/dashboards/my_curriculums"><div class="icon "><i aria-hidden="true" class="fa fa-graduation-cap "></i></div><div class="visible-xs">Curriculums</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-concepts-item" title="Concepts"><a href="/concepts"><div class="icon "><i aria-hidden="true" class="fa fa-file-text "></i></div><div class="visible-xs">Concepts</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-video-rooms" title="Conference rooms"><a href="/dashboards/video_rooms"><div class="icon "><i aria-hidden="true" class="fa fa-comments "></i></div><div class="visible-xs">Conference rooms</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" title="Servers"><a href="/servers"><div class="icon "><i aria-hidden="true" class="fa fa-server "></i></div><div class="visible-xs">Servers</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-my-containers" title="Sandboxes"><a href="/user_containers/current"><div class="icon "><i aria-hidden="true" class="fa fa-terminal "></i></div><div class="visible-xs">Sandboxes</div></a></li>

<li data-container="body" data-placement="right" data-toggle="tooltip" title="Video on demand"><a href="/dashboards/videos"><div class="icon "><i aria-hidden="true" class="fa fa-film "></i></div><div class="visible-xs">Video on demand</div></a></li>

<hr title="My campus">


<li data-container="body" data-placement="right" data-toggle="tooltip" title="Peers"><a href="/users/peers"><div class="icon "><i aria-hidden="true" class="fa fa-users "></i></div><div class="visible-xs">Peers</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" title="Captain&#39;s Logs"><a href="/dashboards/my_captain_log"><div class="icon "><i aria-hidden="true" class="fa fa-book "></i></div><div class="visible-xs">Captain&#39;s Logs</div></a></li>


<hr class="visible-xs">

<li>
<div
data-container="body"
data-placement="right"
data-toggle="tooltip"
title="Slack">
<a target="_blank" href="https://alx-students.slack.com">
<div class="image slack">
<div class="inner"></div>
</div>
<div class="visible-xs">Slack</div>
</a>    </div>

<div
data-container="body"
data-placement="right"
data-toggle="tooltip"
title="My Profile">
<a href="/users/my_profile">
<div class="image ">
<div class="inner" style="background-image: url('https://s3.amazonaws.com/alx-intranet.hbtn.io/users/photos/000/197/885/thumb/joker.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230313%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20230313T084952Z&amp;X-Amz-Expires=600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=db80b9d0b499766c953759d9bcde06f77bd4ebfc2e58d263582f61efabab4314')"></div>
</div>

<div class="visible-xs">My Profile</div>
</a>  </div>
</li>


</ul>
</div>
</nav>

<div class="hidden-xs navigation sidebar">
<a class="logo-container" href="/">
<div class="logo"></div>
</a>
<ul>



<li data-container="body" data-placement="right" data-toggle="tooltip" title="My Planning"><a href="/planning/me"><div class="icon "><i aria-hidden="true" class="fa fa-calendar "></i></div><div class="visible-xs">My Planning</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-current-projects-item" title="Projects"><a href="/projects/current"><div class="icon "><i aria-hidden="true" class="fa fa-code-fork "></i></div><div class="visible-xs">Projects</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" title="QA Reviews I can make"><a href="/corrections/to_review"><div class="icon "><i aria-hidden="true" class="fa fa-check "></i></div><div class="visible-xs">QA Reviews I can make</div></a></li>

<li data-container="body" data-placement="right" data-toggle="tooltip" title="Evaluation quizzes"><a href="/dashboards/my_current_evaluation_quizzes"><div class="icon "><i aria-hidden="true" class="fa fa-question "></i></div><div class="visible-xs">Evaluation quizzes</div></a></li>

<hr title="My resources">

<li data-container="body" data-placement="right" data-toggle="tooltip" title="Curriculums"><a href="/dashboards/my_curriculums"><div class="icon "><i aria-hidden="true" class="fa fa-graduation-cap "></i></div><div class="visible-xs">Curriculums</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-concepts-item" title="Concepts"><a href="/concepts"><div class="icon "><i aria-hidden="true" class="fa fa-file-text "></i></div><div class="visible-xs">Concepts</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-video-rooms" title="Conference rooms"><a href="/dashboards/video_rooms"><div class="icon "><i aria-hidden="true" class="fa fa-comments "></i></div><div class="visible-xs">Conference rooms</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" title="Servers"><a href="/servers"><div class="icon "><i aria-hidden="true" class="fa fa-server "></i></div><div class="visible-xs">Servers</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-my-containers" title="Sandboxes"><a href="/user_containers/current"><div class="icon "><i aria-hidden="true" class="fa fa-terminal "></i></div><div class="visible-xs">Sandboxes</div></a></li>

<li data-container="body" data-placement="right" data-toggle="tooltip" title="Video on demand"><a href="/dashboards/videos"><div class="icon "><i aria-hidden="true" class="fa fa-film "></i></div><div class="visible-xs">Video on demand</div></a></li>

<hr title="My campus">


<li data-container="body" data-placement="right" data-toggle="tooltip" title="Peers"><a href="/users/peers"><div class="icon "><i aria-hidden="true" class="fa fa-users "></i></div><div class="visible-xs">Peers</div></a></li>
<li data-container="body" data-placement="right" data-toggle="tooltip" title="Captain&#39;s Logs"><a href="/dashboards/my_captain_log"><div class="icon "><i aria-hidden="true" class="fa fa-book "></i></div><div class="visible-xs">Captain&#39;s Logs</div></a></li>


<hr class="visible-xs">

<li>
<div
data-container="body"
data-placement="right"
data-toggle="tooltip"
title="Slack">
<a target="_blank" href="https://alx-students.slack.com">
<div class="image slack">
<div class="inner"></div>
</div>
<div class="visible-xs">Slack</div>
</a>    </div>

<div
data-container="body"
data-placement="right"
data-toggle="tooltip"
title="My Profile">
<a href="/users/my_profile">
<div class="image ">
<div class="inner" style="background-image: url('https://s3.amazonaws.com/alx-intranet.hbtn.io/users/photos/000/197/885/thumb/joker.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230313%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20230313T084952Z&amp;X-Amz-Expires=600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=db80b9d0b499766c953759d9bcde06f77bd4ebfc2e58d263582f61efabab4314')"></div>
</div>

<div class="visible-xs">My Profile</div>
</a>  </div>
</li>


</ul>
</div>


<main>
<div id="layout-bars">





</div>

<article class="">


<div class="project row">
<div class="col-xs-12 col-md-10 col-lg-8 contains-images">

<h1 class="gap">0x02. Python - import &amp; modules</h1>

<div data-react-class="tags/Tags" data-react-props="{&quot;tags&quot;:[{&quot;id&quot;:19,&quot;value&quot;:&quot;Python&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;}]}" data-react-cache-id="tags/Tags-0"></div>

<div data-react-class="projects/ProjectMetadata" data-react-props="{&quot;metadata&quot;:{&quot;author&quot;:&quot;Guillaume&quot;,&quot;weight&quot;:1,&quot;correction&quot;:{&quot;released&quot;:true,&quot;requires_auto_correction&quot;:true,&quot;requires_manual_correction&quot;:false},&quot;bpi&quot;:{&quot;current&quot;:false,&quot;in_second_deadline&quot;:true,&quot;starts_at&quot;:&quot;2023-03-09T06:00:00.000+03:00&quot;,&quot;ends_at&quot;:&quot;2023-03-10T06:00:00.000+03:00&quot;,&quot;second_deadline_at&quot;:&quot;2023-03-16T06:00:00.000+03:00&quot;}}}" data-react-cache-id="projects/ProjectMetadata-0"></div>

<div class="sm-gap clean well">
<h4>In a nutshell&hellip;</h4>
<ul>


<li>
<strong>Auto QA review:</strong>
0.0/85 mandatory
&
0.0/58 optional
</li>
<li>
<strong>Altogether:</strong>
&nbsp;<strong>0.0%</strong>
<ul>
<li>Mandatory: 0.0%</li>
<li>Optional: 0.0%</li>
<li>
Calculation:&nbsp;
0.0%
+ (0.0% * 0.0%)
&nbsp;==&nbsp;<strong>0.0%</strong>
</li>
</ul>
</li>
</ul>
</div>







<div id="project_id" style="display: none" data-project-id="239"></div>







<div class="panel panel-default" id="project-description">
<div class="panel-body">
<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="/rltoken/SY-cMfnwbHoPFaJ-D_LWig" title="Modules" target="_blank">Modules</a> </li>
<li><a href="/rltoken/5e3TphtJ6WSVkWsdd2eX_A" title="Command line arguments" target="_blank">Command line arguments</a> </li>
<li><a href="/rltoken/FlkAJ_kPXHC4Y65WrRvA4A" title="Pycodestyle -- Style Guide for Python Code" target="_blank">Pycodestyle &ndash; Style Guide for Python Code</a> </li>
</ul>

<p><strong>man or help</strong>:</p>

<ul>
<li><code>python3</code></li>
</ul>

<h2>Learning Objectives</h2>

<p>At the end of this project, you are expected to be able to <a href="/rltoken/wwTE_cGg7Ug-Vp3IQ6tmXA" title="explain to anyone" target="_blank">explain to anyone</a>, <strong>without the help of Google</strong>:</p>

<h3>General</h3>

<ul>
<li>Why Python programming is awesome</li>
<li>How to import functions from another file</li>
<li>How to use imported functions</li>
<li>How to create a module</li>
<li>How to use the built-in function <code>dir()</code></li>
<li>How to prevent code in your script from being executed when imported</li>
<li>How to use command line arguments with your Python programs</li>
</ul>

<h3>Copyright - Plagiarism</h3>

<ul>
<li>You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.</li>
<li>You will not be able to meet the objectives of this or any following project by copying and pasting someone else&rsquo;s work. </li>
<li>You are not allowed to publish any content of this project.</li>
<li>Any form of plagiarism is strictly forbidden and will result in removal from the program.</li>
</ul>

<h2>Requirements</h2>

<h3>General</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)</li>
<li>All your files should end with a new line</li>
<li>The first line of all your files should be exactly <code>#!/usr/bin/python3</code></li>
<li>A <code>README.md</code> file, at the root of the folder of the project, is mandatory</li>
<li>Your code should use the pycodestyle (version <code>2.8.*</code>)</li>
<li>All your files must be executable</li>
<li>The length of your files will be tested using <code>wc</code></li>
</ul>

</div>
</div>




<div class="panel panel-default" id="project-quiz-questions-title">
<div class="panel-heading">
<h3 class="panel-title">
Quiz questions
</h3>
</div>

<div class="panel-body">

<div class="alert alert-info">
<strong>Great!</strong>
You've completed the quiz successfully! Keep going!
<span id="quiz_questions_collapse_toggle"></span>
</div>

<section class="quiz_questions_show_container">
<div class="quiz_question_item_container" data-role="quiz_question227" data-position="3">
<div class=" clearfix" id="quiz_question-227">

<h4 class="quiz_question">

Question #0
</h4>

<!-- Quiz question Body -->
<p>What do these lines print?</p>

<pre><code>&gt;&gt;&gt; def my_function(counter):
&gt;&gt;&gt;     print(&quot;Counter: {}&quot;.format(counter))
&gt;&gt;&gt; 
&gt;&gt;&gt; my_function(12)
</code></pre>


<!-- Quiz question Answers -->
<ul class="quiz_question_answers" data-question-id="227">
<li class="">

<input type="radio" name="227" id="227-1501189497109" value="1501189497109" data-quiz-answer-id="1501189497109" data-quiz-question-id="227" disabled="disabled" />
<label for="227-1501189497109"><p>Counter: counter</p>
</label>
</li>

<li class="">

<input type="radio" name="227" id="227-1501189541820" value="1501189541820" data-quiz-answer-id="1501189541820" data-quiz-question-id="227" disabled="disabled" checked="checked" />
<label for="227-1501189541820"><p>Counter: 12</p>
</label>
</li>

<li class="">

<input type="radio" name="227" id="227-1501189537703" value="1501189537703" data-quiz-answer-id="1501189537703" data-quiz-question-id="227" disabled="disabled" />
<label for="227-1501189537703"><p>Counter: c</p>
</label>
</li>

</ul>

<!-- Quiz question Tips -->

</div>

</div>
<div class="quiz_question_item_container" data-role="quiz_question228" data-position="4">
<div class=" clearfix" id="quiz_question-228">

<h4 class="quiz_question">

Question #1
</h4>

<!-- Quiz question Body -->
<p>What do these lines print?</p>

<pre><code>&gt;&gt;&gt; def my_function(counter=89):
&gt;&gt;&gt;     print(&quot;Counter: {}&quot;.format(counter))
&gt;&gt;&gt; 
&gt;&gt;&gt; my_function(12)
</code></pre>


<!-- Quiz question Answers -->
<ul class="quiz_question_answers" data-question-id="228">
<li class="">

<input type="radio" name="228" id="228-1501189549558" value="1501189549558" data-quiz-answer-id="1501189549558" data-quiz-question-id="228" disabled="disabled" checked="checked" />
<label for="228-1501189549558"><p>Counter: 12</p>
</label>
</li>

<li class="">

<input type="radio" name="228" id="228-1501189561657" value="1501189561657" data-quiz-answer-id="1501189561657" data-quiz-question-id="228" disabled="disabled" />
<label for="228-1501189561657"><p>Counter: 101</p>
</label>
</li>

<li class="">

<input type="radio" name="228" id="228-1501189556222" value="1501189556222" data-quiz-answer-id="1501189556222" data-quiz-question-id="228" disabled="disabled" />
<label for="228-1501189556222"><p>Counter: 89</p>
</label>
</li>

</ul>

<!-- Quiz question Tips -->

</div>

</div>
<div class="quiz_question_item_container" data-role="quiz_question225" data-position="1">
<div class=" clearfix" id="quiz_question-225">

<h4 class="quiz_question">

Question #2
</h4>

<!-- Quiz question Body -->
<p>What do these lines print?</p>

<pre><code>&gt;&gt;&gt; def my_function():
&gt;&gt;&gt;     print(&quot;In my function&quot;)
&gt;&gt;&gt; 
&gt;&gt;&gt; my_function()
</code></pre>


<!-- Quiz question Answers -->
<ul class="quiz_question_answers" data-question-id="225">
<li class="">

<input type="radio" name="225" id="225-1501189284630" value="1501189284630" data-quiz-answer-id="1501189284630" data-quiz-question-id="225" disabled="disabled" />
<label for="225-1501189284630"><p>function my_function at &hellip;</p>
</label>
</li>

<li class="">

<input type="radio" name="225" id="225-1501189274816" value="1501189274816" data-quiz-answer-id="1501189274816" data-quiz-question-id="225" disabled="disabled" />
<label for="225-1501189274816"><p>&ldquo;In my function&rdquo;</p>
</label>
</li>

<li class="">

<input type="radio" name="225" id="225-1501189347459" value="1501189347459" data-quiz-answer-id="1501189347459" data-quiz-question-id="225" disabled="disabled" />
<label for="225-1501189347459"><p>Nothing</p>
</label>
</li>

<li class="">

<input type="radio" name="225" id="225-1501189280027" value="1501189280027" data-quiz-answer-id="1501189280027" data-quiz-question-id="225" disabled="disabled" checked="checked" />
<label for="225-1501189280027"><p>In my function</p>
</label>
</li>

</ul>

<!-- Quiz question Tips -->

</div>

</div>
<div class="quiz_question_item_container" data-role="quiz_question229" data-position="5">
<div class=" clearfix" id="quiz_question-229">

<h4 class="quiz_question">

Question #3
</h4>

<!-- Quiz question Body -->
<p>What do these lines print?</p>

<pre><code>&gt;&gt;&gt; def my_function(counter=89):
&gt;&gt;&gt;     print(&quot;Counter: {}&quot;.format(counter))
&gt;&gt;&gt; 
&gt;&gt;&gt; my_function()
</code></pre>


<!-- Quiz question Answers -->
<ul class="quiz_question_answers" data-question-id="229">
<li class="">

<input type="radio" name="229" id="229-1501189576821" value="1501189576821" data-quiz-answer-id="1501189576821" data-quiz-question-id="229" disabled="disabled" />
<label for="229-1501189576821"><p>Counter: 12</p>
</label>
</li>

<li class="">

<input type="radio" name="229" id="229-1501189587800" value="1501189587800" data-quiz-answer-id="1501189587800" data-quiz-question-id="229" disabled="disabled" />
<label for="229-1501189587800"><p>Counter: 101</p>
</label>
</li>

<li class="">

<input type="radio" name="229" id="229-1501189580406" value="1501189580406" data-quiz-answer-id="1501189580406" data-quiz-question-id="229" disabled="disabled" checked="checked" />
<label for="229-1501189580406"><p>Counter: 89</p>
</label>
</li>

</ul>

<!-- Quiz question Tips -->

</div>

</div>
<div class="quiz_question_item_container" data-role="quiz_question230" data-position="6">
<div class=" clearfix" id="quiz_question-230">

<h4 class="quiz_question">

Question #4
</h4>

<!-- Quiz question Body -->
<p>What do these lines print?</p>

<pre><code>&gt;&gt;&gt; def my_function(counter=89):
&gt;&gt;&gt;     return counter + 1
&gt;&gt;&gt; 
&gt;&gt;&gt; print(my_function())
</code></pre>


<!-- Quiz question Answers -->
<ul class="quiz_question_answers" data-question-id="230">
<li class="">

<input type="radio" name="230" id="230-1501189604081" value="1501189604081" data-quiz-answer-id="1501189604081" data-quiz-question-id="230" disabled="disabled" checked="checked" />
<label for="230-1501189604081"><p>90</p>
</label>
</li>

<li class="">

<input type="radio" name="230" id="230-1501189597435" value="1501189597435" data-quiz-answer-id="1501189597435" data-quiz-question-id="230" disabled="disabled" />
<label for="230-1501189597435"><p>1</p>
</label>
</li>

<li class="">

<input type="radio" name="230" id="230-1501189609366" value="1501189609366" data-quiz-answer-id="1501189609366" data-quiz-question-id="230" disabled="disabled" />
<label for="230-1501189609366"><p>891</p>
</label>
</li>

<li class="">

<input type="radio" name="230" id="230-1501189601403" value="1501189601403" data-quiz-answer-id="1501189601403" data-quiz-question-id="230" disabled="disabled" />
<label for="230-1501189601403"><p>89</p>
</label>
</li>

</ul>

<!-- Quiz question Tips -->

</div>

</div>
<div class="quiz_question_item_container" data-role="quiz_question226" data-position="2">
<div class=" clearfix" id="quiz_question-226">

<h4 class="quiz_question">

Question #5
</h4>

<!-- Quiz question Body -->
<p>What do these lines print?</p>

<pre><code>&gt;&gt;&gt; def my_function():
&gt;&gt;&gt;     print(&quot;In my function&quot;)
&gt;&gt;&gt; 
&gt;&gt;&gt; my_function
</code></pre>


<!-- Quiz question Answers -->
<ul class="quiz_question_answers" data-question-id="226">
<li class="">

<input type="radio" name="226" id="226-1501189361826" value="1501189361826" data-quiz-answer-id="1501189361826" data-quiz-question-id="226" disabled="disabled" checked="checked" />
<label for="226-1501189361826"><p>function my_function at &hellip;</p>
</label>
</li>

<li class="">

<input type="radio" name="226" id="226-1501189355769" value="1501189355769" data-quiz-answer-id="1501189355769" data-quiz-question-id="226" disabled="disabled" />
<label for="226-1501189355769"><p>&ldquo;In my function&rdquo;</p>
</label>
</li>

<li class="">

<input type="radio" name="226" id="226-1501189372306" value="1501189372306" data-quiz-answer-id="1501189372306" data-quiz-question-id="226" disabled="disabled" />
<label for="226-1501189372306"><p>Nothing</p>
</label>
</li>

<li class="">

<input type="radio" name="226" id="226-1501189357670" value="1501189357670" data-quiz-answer-id="1501189357670" data-quiz-question-id="226" disabled="disabled" />
<label for="226-1501189357670"><p>In my function</p>
</label>
</li>

</ul>

<!-- Quiz question Tips -->

</div>

</div>

</section>
</div>
</div>



<h2 class="gap">Tasks</h2>

<div data-role="task1083" data-position="1" id="task-num-0">
<div class="panel panel-default task-card " id="task-1083">
<span id="user_id" data-id="197885"></span>

<div class="panel-heading panel-heading-actions">
<h3 class="panel-title">
0. Import a simple function from a simple file
</h3>

<div>
<span class="label label-info">
mandatory
</span>
</div>
</div>

<div class="panel-body">
<span id="user_id" data-id="197885"></span>

<!-- Progress vs Score -->
<div class="task_progress_score_bar" data-task-id="1083" data-correction-id="12737951">
<div class="task_progress_bar" style="width: 0.0%">
<div class="task_score_bar" style="width: NaN%">
</div>
</div>
<div class="task_progress_score_text">
Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
</div>
</div>

<!-- Task Body -->
<p>Write a program that imports the function <code>def add(a, b):</code> from the file <code>add_0.py</code> and prints the result of the addition <code>1 + 2 = 3</code></p>

<ul>
<li>You have to use <code>print</code> function with string format to display integers</li>
<li>You have to assign:

<ul>
<li>the value <code>1</code> to a variable called <code>a</code> </li>
<li>the value <code>2</code> to a variable called <code>b</code></li>
<li>and use those two variables as arguments when calling the functions <code>add</code> and <code>print</code></li>
</ul></li>
<li><code>a</code> and <code>b</code> must be defined in 2 different lines: <code>a = 1</code> and another <code>b = 2</code></li>
<li>Your program should print: <code>&lt;a value&gt; + &lt;b value&gt; = &lt;add(a, b) value&gt;</code> followed with a new line</li>
<li>You can only use the word <code>add_0</code> once in your code</li>
<li>You are not allowed to use <code>*</code> for importing or <code>__import__</code></li>
<li>Your code should not be executed when imported - by using <code>__import__</code>, like the example below</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x02$ cat add_0.py
#!/usr/bin/python3
def add(a, b):
&quot;&quot;&quot;My addition function

Args:
a: first integer
b: second integer

Returns:
The return value. a + b
&quot;&quot;&quot;
return (a + b)

guillaume@ubuntu:~/0x02$ ./0-add.py
1 + 2 = 3
guillaume@ubuntu:~/0x02$ cat 0-import_add.py
__import__(&quot;0-add&quot;)
guillaume@ubuntu:~/0x02$ python3 0-import_add.py 
guillaume@ubuntu:~/0x02$ 
</code></pre>

</div>

<div class="list-group">
<!-- Task URLs -->

<!-- Github information -->
<div class="list-group-item">
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>alx-higher_level_programming</code></li>
<li>Directory: <code>0x02-python-import_modules</code></li>
<li>File: <code>0-add.py</code></li>
</ul>
</div>

<!-- Self-paced manual review -->
</div>

<!-- Panel footer - Controls -->
<div class="panel-footer">
<div class="align-items-center d-flex justify-content-between">

<div>
<button class="student_task_done btn btn-default btn-sm no" data-task-id="1083">
<span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
<span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
<span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
Done<span class="no pending">?</span><span class="yes">!</span>
</button>

<button class="student-task-done-by btn btn-default btn-sm" data-task-id="1083" data-batch-id="26" data-toggle="modal" data-target="#task-1083-users-done-modal">
Help
</button>
<div class="modal fade users-done-modal" id="task-1083-users-done-modal" data-task-id="1083" data-batch-id="26">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Students who are done with "0. Import a simple function from a simple file"</h4>
</div>
<div class="modal-body">
<div class="list-group">
</div>
<div class="spinner">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
</div>
</div>
</div>
</div>


<button class="btn btn-default btn-sm check-your-task-1083-modal-button" data-task-id="1083" data-toggle="modal" data-target="#task-test-correction-1083-correction-modal" id="task-num-0-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1083}'>
Check your code
</button>
<div class="modal fade task_correction_modal student_modal" id="task-test-correction-1083-correction-modal">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Correction of "0. Import a simple function from a simple file"</h4>
</div>
<div class="modal-body">
<div class="actions">
<center>
<div class="alert alert-info hidden"></div>

<button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1083">Start a new test</button>
<button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

<div class="spinner" style="display: none;">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
<div class="info"></div>
</center>
</div>
<div class="result"></div>

<div class="help">
<button data-task-id="1083">
<i aria-hidden="true" class="fa fa-info-circle "></i>
</button>
<div class="help-container" data-task-id="1083">
<div class="check-line">
<div class="check-inline requirement success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Requirement success
</div>
<div class="check-inline requirement fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Requirement fail
</div>
</div>
<div class="check-line">
<div class="check-inline code success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Code success
</div>
<div class="check-inline code fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Code fail
</div>
</div>
<div class="check-line">
<div class="check-inline efficiency success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Efficiency success
</div>
<div class="check-inline efficiency fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Efficiency fail
</div>
</div>
<div class="check-line">
<div class="check-inline answer success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Text answer success
</div>
<div class="check-inline answer fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Text answer fail
</div>
</div>
<div class="check-line">
<div class="check-inline requirement fail offline">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Skipped - Previous check failed
</div>
</div>
</div>
</div>

</div>
</div>
</div>
</div>



<button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1083}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

<button class="btn btn-default btn-sm" data-task-id="1083" data-toggle="modal" data-target="#task-qa-review-1083-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1083}'>
QA Review
</button>
<div class="modal fade task_get_qa_review" id="task-qa-review-1083-modal" data-correction-id="12737951" data-task-id="1083">
<div class="modal-dialog modal-lg">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">0. Import a simple function from a simple file</h4>
</div>
<div class="modal-body">
<div class="spinner gap">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="review-container">
<div class="review-corrector"></div>
<div class="review-github well" style="display:none">
<h5>Commit used:</h5>
<ul>
<li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
<li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
<li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
<li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
<li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
<li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
</ul>
</div>
<div class="review-percentage_down"></div>
<ul class="review-checks list-group sm-gap"></ul>
<div class="review-comment"></div>
</div>
</div>
</div>
</div>
</div>

</div>


<div class="fs-4">
</div>
</div>


</div>
</div>

</div>
<div data-role="task1084" data-position="2" id="task-num-1">
<div class="panel panel-default task-card " id="task-1084">
<span id="user_id" data-id="197885"></span>

<div class="panel-heading panel-heading-actions">
<h3 class="panel-title">
1. My first toolbox!
</h3>

<div>
<span class="label label-info">
mandatory
</span>
</div>
</div>

<div class="panel-body">
<span id="user_id" data-id="197885"></span>

<!-- Progress vs Score -->
<div class="task_progress_score_bar" data-task-id="1084" data-correction-id="12737951">
<div class="task_progress_bar" style="width: 0.0%">
<div class="task_score_bar" style="width: NaN%">
</div>
</div>
<div class="task_progress_score_text">
Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
</div>
</div>

<!-- Task Body -->
<p>Write a program that imports functions from the file <code>calculator_1.py</code>, does some Maths, and prints the result.</p>

<ul>
<li>Do not use the function <code>print</code> (with string format to display integers) more than 4 times </li>
<li>You have to define:

<ul>
<li>the value <code>10</code> to a variable <code>a</code></li>
<li>the value <code>5</code> to a variable <code>b</code></li>
<li>and use those two variables only, as arguments when calling functions (including <code>print</code>)</li>
</ul></li>
<li><code>a</code> and <code>b</code> must be defined in 2 different lines: <code>a = 10</code> and another <code>b = 5</code></li>
<li>Your program should call each of the imported functions. See example below for format</li>
<li>the word <code>calculator_1</code> should be used only once in your file</li>
<li>You are not allowed to use <code>*</code> for importing or <code>__import__</code></li>
<li>Your code should not be executed when imported</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x02$ cat calculator_1.py
#!/usr/bin/python3
def add(a, b):
&quot;&quot;&quot;My addition function

Args:
a: first integer
b: second integer

Returns:
The return value. a + b
&quot;&quot;&quot;
return (a + b)


def sub(a, b):
&quot;&quot;&quot;My subtraction function

Args:
a: first integer
b: second integer

Returns:
The return value. a - b
&quot;&quot;&quot;
return (a - b)


def mul(a, b):
&quot;&quot;&quot;My multiplication function

Args:
a: first integer
b: second integer

Returns:
The return value. a * b
&quot;&quot;&quot;
return (a * b)


def div(a, b):
&quot;&quot;&quot;My division function

Args:
a: first integer
b: second integer

Returns:
The return value. a / b
&quot;&quot;&quot;
return int(a / b)

guillaume@ubuntu:~/0x02$ ./1-calculation.py
10 + 5 = 15
10 - 5 = 5
10 * 5 = 50
10 / 5 = 2
guillaume@ubuntu:~/0x02$
</code></pre>

</div>

<div class="list-group">
<!-- Task URLs -->

<!-- Github information -->
<div class="list-group-item">
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>alx-higher_level_programming</code></li>
<li>Directory: <code>0x02-python-import_modules</code></li>
<li>File: <code>1-calculation.py</code></li>
</ul>
</div>

<!-- Self-paced manual review -->
</div>

<!-- Panel footer - Controls -->
<div class="panel-footer">
<div class="align-items-center d-flex justify-content-between">

<div>
<button class="student_task_done btn btn-default btn-sm no" data-task-id="1084">
<span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
<span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
<span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
Done<span class="no pending">?</span><span class="yes">!</span>
</button>

<button class="student-task-done-by btn btn-default btn-sm" data-task-id="1084" data-batch-id="26" data-toggle="modal" data-target="#task-1084-users-done-modal">
Help
</button>
<div class="modal fade users-done-modal" id="task-1084-users-done-modal" data-task-id="1084" data-batch-id="26">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Students who are done with "1. My first toolbox!"</h4>
</div>
<div class="modal-body">
<div class="list-group">
</div>
<div class="spinner">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
</div>
</div>
</div>
</div>


<button class="btn btn-default btn-sm check-your-task-1084-modal-button" data-task-id="1084" data-toggle="modal" data-target="#task-test-correction-1084-correction-modal" id="task-num-1-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1084}'>
Check your code
</button>
<div class="modal fade task_correction_modal student_modal" id="task-test-correction-1084-correction-modal">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Correction of "1. My first toolbox!"</h4>
</div>
<div class="modal-body">
<div class="actions">
<center>
<div class="alert alert-info hidden"></div>

<button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1084">Start a new test</button>
<button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

<div class="spinner" style="display: none;">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
<div class="info"></div>
</center>
</div>
<div class="result"></div>

<div class="help">
<button data-task-id="1084">
<i aria-hidden="true" class="fa fa-info-circle "></i>
</button>
<div class="help-container" data-task-id="1084">
<div class="check-line">
<div class="check-inline requirement success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Requirement success
</div>
<div class="check-inline requirement fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Requirement fail
</div>
</div>
<div class="check-line">
<div class="check-inline code success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Code success
</div>
<div class="check-inline code fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Code fail
</div>
</div>
<div class="check-line">
<div class="check-inline efficiency success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Efficiency success
</div>
<div class="check-inline efficiency fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Efficiency fail
</div>
</div>
<div class="check-line">
<div class="check-inline answer success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Text answer success
</div>
<div class="check-inline answer fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Text answer fail
</div>
</div>
<div class="check-line">
<div class="check-inline requirement fail offline">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Skipped - Previous check failed
</div>
</div>
</div>
</div>

</div>
</div>
</div>
</div>



<button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1084}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

<button class="btn btn-default btn-sm" data-task-id="1084" data-toggle="modal" data-target="#task-qa-review-1084-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1084}'>
QA Review
</button>
<div class="modal fade task_get_qa_review" id="task-qa-review-1084-modal" data-correction-id="12737951" data-task-id="1084">
<div class="modal-dialog modal-lg">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">1. My first toolbox!</h4>
</div>
<div class="modal-body">
<div class="spinner gap">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="review-container">
<div class="review-corrector"></div>
<div class="review-github well" style="display:none">
<h5>Commit used:</h5>
<ul>
<li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
<li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
<li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
<li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
<li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
<li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
</ul>
</div>
<div class="review-percentage_down"></div>
<ul class="review-checks list-group sm-gap"></ul>
<div class="review-comment"></div>
</div>
</div>
</div>
</div>
</div>

</div>


<div class="fs-4">
</div>
</div>


</div>
</div>

</div>
<div data-role="task1085" data-position="3" id="task-num-2">
<div class="panel panel-default task-card " id="task-1085">
<span id="user_id" data-id="197885"></span>

<div class="panel-heading panel-heading-actions">
<h3 class="panel-title">
2. How to make a script dynamic!
</h3>

<div>
<span class="label label-info">
mandatory
</span>
</div>
</div>

<div class="panel-body">
<span id="user_id" data-id="197885"></span>

<!-- Progress vs Score -->
<div class="task_progress_score_bar" data-task-id="1085" data-correction-id="12737951">
<div class="task_progress_bar" style="width: 0.0%">
<div class="task_score_bar" style="width: NaN%">
</div>
</div>
<div class="task_progress_score_text">
Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
</div>
</div>

<!-- Task Body -->
<p>Write a program that prints the number of and the list of its arguments.</p>

<ul>
<li>The output should be:

<ul>
<li>Number of argument(s) followed by <code>argument</code> (if number is one) or <code>arguments</code> (otherwise), followed by</li>
<li><code>:</code> (or <code>.</code> if no arguments were passed) followed by</li>
<li>a new line, followed by (if at least one argument),</li>
<li>one line per argument:

<ul>
<li>the position of the argument (starting at <code>1</code>) followed by <code>:</code>, followed by the argument value and a new line</li>
</ul></li>
</ul></li>
<li>Your code should not be executed when imported</li>
<li>The number of elements of <code>argv</code> can be retrieved by using: <code>len(argv)</code></li>
<li>You do not have to fully understand lists yet, but imagine that <code>argv</code> can be used just like a C array: you can use an index to walk through it. There are other ways (which will be preferred for future project tasks), if you know them you can use them.</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x02$ ./2-args.py 
0 arguments.
guillaume@ubuntu:~/0x02$ ./2-args.py Hello
1 argument:
1: Hello
guillaume@ubuntu:~/0x02$ ./2-args.py Hello Welcome To The Best School
6 arguments:
1: Hello
2: Welcome
3: To
4: The
5: Best
6: School
guillaume@ubuntu:~/0x02$ 
</code></pre>

</div>

<div class="list-group">
<!-- Task URLs -->

<!-- Github information -->
<div class="list-group-item">
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>alx-higher_level_programming</code></li>
<li>Directory: <code>0x02-python-import_modules</code></li>
<li>File: <code>2-args.py</code></li>
</ul>
</div>

<!-- Self-paced manual review -->
</div>

<!-- Panel footer - Controls -->
<div class="panel-footer">
<div class="align-items-center d-flex justify-content-between">

<div>
<button class="student_task_done btn btn-default btn-sm no" data-task-id="1085">
<span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
<span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
<span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
Done<span class="no pending">?</span><span class="yes">!</span>
</button>

<button class="student-task-done-by btn btn-default btn-sm" data-task-id="1085" data-batch-id="26" data-toggle="modal" data-target="#task-1085-users-done-modal">
Help
</button>
<div class="modal fade users-done-modal" id="task-1085-users-done-modal" data-task-id="1085" data-batch-id="26">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Students who are done with "2. How to make a script dynamic!"</h4>
</div>
<div class="modal-body">
<div class="list-group">
</div>
<div class="spinner">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
</div>
</div>
</div>
</div>


<button class="btn btn-default btn-sm check-your-task-1085-modal-button" data-task-id="1085" data-toggle="modal" data-target="#task-test-correction-1085-correction-modal" id="task-num-2-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1085}'>
Check your code
</button>
<div class="modal fade task_correction_modal student_modal" id="task-test-correction-1085-correction-modal">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Correction of "2. How to make a script dynamic!"</h4>
</div>
<div class="modal-body">
<div class="actions">
<center>
<div class="alert alert-info hidden"></div>

<button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1085">Start a new test</button>
<button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

<div class="spinner" style="display: none;">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
<div class="info"></div>
</center>
</div>
<div class="result"></div>

<div class="help">
<button data-task-id="1085">
<i aria-hidden="true" class="fa fa-info-circle "></i>
</button>
<div class="help-container" data-task-id="1085">
<div class="check-line">
<div class="check-inline requirement success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Requirement success
</div>
<div class="check-inline requirement fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Requirement fail
</div>
</div>
<div class="check-line">
<div class="check-inline code success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Code success
</div>
<div class="check-inline code fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Code fail
</div>
</div>
<div class="check-line">
<div class="check-inline efficiency success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Efficiency success
</div>
<div class="check-inline efficiency fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Efficiency fail
</div>
</div>
<div class="check-line">
<div class="check-inline answer success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Text answer success
</div>
<div class="check-inline answer fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Text answer fail
</div>
</div>
<div class="check-line">
<div class="check-inline requirement fail offline">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Skipped - Previous check failed
</div>
</div>
</div>
</div>

</div>
</div>
</div>
</div>



<button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1085}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

<button class="btn btn-default btn-sm" data-task-id="1085" data-toggle="modal" data-target="#task-qa-review-1085-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1085}'>
QA Review
</button>
<div class="modal fade task_get_qa_review" id="task-qa-review-1085-modal" data-correction-id="12737951" data-task-id="1085">
<div class="modal-dialog modal-lg">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">2. How to make a script dynamic!</h4>
</div>
<div class="modal-body">
<div class="spinner gap">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="review-container">
<div class="review-corrector"></div>
<div class="review-github well" style="display:none">
<h5>Commit used:</h5>
<ul>
<li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
<li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
<li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
<li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
<li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
<li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
</ul>
</div>
<div class="review-percentage_down"></div>
<ul class="review-checks list-group sm-gap"></ul>
<div class="review-comment"></div>
</div>
</div>
</div>
</div>
</div>

</div>


<div class="fs-4">
</div>
</div>


</div>
</div>

</div>
<div data-role="task1086" data-position="4" id="task-num-3">
<div class="panel panel-default task-card " id="task-1086">
<span id="user_id" data-id="197885"></span>

<div class="panel-heading panel-heading-actions">
<h3 class="panel-title">
3. Infinite addition
</h3>

<div>
<span class="label label-info">
mandatory
</span>
</div>
</div>

<div class="panel-body">
<span id="user_id" data-id="197885"></span>

<!-- Progress vs Score -->
<div class="task_progress_score_bar" data-task-id="1086" data-correction-id="12737951">
<div class="task_progress_bar" style="width: 0.0%">
<div class="task_score_bar" style="width: NaN%">
</div>
</div>
<div class="task_progress_score_text">
Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
</div>
</div>

<!-- Task Body -->
<p>Write a program that prints the result of the addition of all arguments</p>

<ul>
<li>The output should be the result of the addition of all arguments, followed by a new line</li>
<li>You can cast arguments into integers by using <code>int()</code> (you can assume that all arguments can be casted into integers)</li>
<li>Your code should not be executed when imported</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x02$ ./3-infinite_add.py
0
guillaume@ubuntu:~/0x02$ ./3-infinite_add.py 79 10
89
guillaume@ubuntu:~/0x02$ ./3-infinite_add.py 79 10 -40 -300 89 
-162
guillaume@ubuntu:~/0x02$ 
</code></pre>

<p>Last but not least, your program should also handle big numbers. And the good news is: if your program works for the above example, it will work for the following example:</p>

<pre><code>guillaume@ubuntu:~/0x02$ ./3-infinite_add.py 1111111111111111111111111111111111111111111111111111111111112222222222222222222222222222222222223435467866765443534434222222254444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555666666666666666666666666666666777777777777777777777777777777888888888888888888888888888888899999999999999999999999990000000000000000000 11111111111111111111111111111111111111111111111111222222222222222222222222222333333333333333333334567788888899999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
11111111111111111111111111111111111111111111111111222222222222222222222222222333333333333333333334568900000011111111111111111111111111111111111111111111111111112222222222222222222222222222222222223435467866765443534434222222254444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444444555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555555666666666666666666666666666666777777777777777777777777777777888888888888888888888888888888899999999999999999999999989999999999999999999
guillaume@ubuntu:~/0x02$
</code></pre>

<p>Remember how you did (or did not) do it in C? <code>#pythoniscool</code></p>

<p><img src="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/621c6dd72e1acff708141f3fab6dfa6ff37c5ee6.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230313%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230313T084952Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=84c0d948a3d747d3549390d0ce52033ff1a9c90c0053a7ba67c1637a7cc5fcbc" alt="" loading='lazy' style="" /></p>

</div>

<div class="list-group">
<!-- Task URLs -->

<!-- Github information -->
<div class="list-group-item">
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>alx-higher_level_programming</code></li>
<li>Directory: <code>0x02-python-import_modules</code></li>
<li>File: <code>3-infinite_add.py</code></li>
</ul>
</div>

<!-- Self-paced manual review -->
</div>

<!-- Panel footer - Controls -->
<div class="panel-footer">
<div class="align-items-center d-flex justify-content-between">

<div>
<button class="student_task_done btn btn-default btn-sm no" data-task-id="1086">
<span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
<span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
<span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
Done<span class="no pending">?</span><span class="yes">!</span>
</button>

<button class="student-task-done-by btn btn-default btn-sm" data-task-id="1086" data-batch-id="26" data-toggle="modal" data-target="#task-1086-users-done-modal">
Help
</button>
<div class="modal fade users-done-modal" id="task-1086-users-done-modal" data-task-id="1086" data-batch-id="26">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Students who are done with "3. Infinite addition"</h4>
</div>
<div class="modal-body">
<div class="list-group">
</div>
<div class="spinner">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
</div>
</div>
</div>
</div>


<button class="btn btn-default btn-sm check-your-task-1086-modal-button" data-task-id="1086" data-toggle="modal" data-target="#task-test-correction-1086-correction-modal" id="task-num-3-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1086}'>
Check your code
</button>
<div class="modal fade task_correction_modal student_modal" id="task-test-correction-1086-correction-modal">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Correction of "3. Infinite addition"</h4>
</div>
<div class="modal-body">
<div class="actions">
<center>
<div class="alert alert-info hidden"></div>

<button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1086">Start a new test</button>
<button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

<div class="spinner" style="display: none;">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
<div class="info"></div>
</center>
</div>
<div class="result"></div>

<div class="help">
<button data-task-id="1086">
<i aria-hidden="true" class="fa fa-info-circle "></i>
</button>
<div class="help-container" data-task-id="1086">
<div class="check-line">
<div class="check-inline requirement success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Requirement success
</div>
<div class="check-inline requirement fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Requirement fail
</div>
</div>
<div class="check-line">
<div class="check-inline code success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Code success
</div>
<div class="check-inline code fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Code fail
</div>
</div>
<div class="check-line">
<div class="check-inline efficiency success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Efficiency success
</div>
<div class="check-inline efficiency fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Efficiency fail
</div>
</div>
<div class="check-line">
<div class="check-inline answer success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Text answer success
</div>
<div class="check-inline answer fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Text answer fail
</div>
</div>
<div class="check-line">
<div class="check-inline requirement fail offline">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Skipped - Previous check failed
</div>
</div>
</div>
</div>

</div>
</div>
</div>
</div>



<button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1086}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

<button class="btn btn-default btn-sm" data-task-id="1086" data-toggle="modal" data-target="#task-qa-review-1086-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1086}'>
QA Review
</button>
<div class="modal fade task_get_qa_review" id="task-qa-review-1086-modal" data-correction-id="12737951" data-task-id="1086">
<div class="modal-dialog modal-lg">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">3. Infinite addition</h4>
</div>
<div class="modal-body">
<div class="spinner gap">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="review-container">
<div class="review-corrector"></div>
<div class="review-github well" style="display:none">
<h5>Commit used:</h5>
<ul>
<li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
<li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
<li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
<li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
<li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
<li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
</ul>
</div>
<div class="review-percentage_down"></div>
<ul class="review-checks list-group sm-gap"></ul>
<div class="review-comment"></div>
</div>
</div>
</div>
</div>
</div>

</div>


<div class="fs-4">
</div>
</div>


</div>
</div>

</div>
<div data-role="task1087" data-position="5" id="task-num-4">
<div class="panel panel-default task-card " id="task-1087">
<span id="user_id" data-id="197885"></span>

<div class="panel-heading panel-heading-actions">
<h3 class="panel-title">
4. Who are you?
</h3>

<div>
<span class="label label-info">
mandatory
</span>
</div>
</div>

<div class="panel-body">
<span id="user_id" data-id="197885"></span>

<!-- Progress vs Score -->
<div class="task_progress_score_bar" data-task-id="1087" data-correction-id="12737951">
<div class="task_progress_bar" style="width: 0.0%">
<div class="task_score_bar" style="width: NaN%">
</div>
</div>
<div class="task_progress_score_text">
Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
</div>
</div>

<!-- Task Body -->
<p>Write a program that prints all the names defined by the compiled module <a href="https://github.com/holbertonschool/0x02.py/raw/master/hidden_4.pyc" title="hidden_4.pyc" target="_blank">hidden_4.pyc</a> (please download it locally).</p>

<ul>
<li>You should print one name per line, in alpha order</li>
<li>You should print only names that do <strong>not</strong> start with <code>__</code></li>
<li>Your code should not be executed when imported</li>
<li>Make sure you are running your code in Python3.8.x (<code>hidden_4.pyc</code> has been compiled with this version)</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x02$ curl -Lso &quot;hidden_4.pyc&quot; &quot;https://github.com/holbertonschool/0x02.py/raw/master/hidden_4.pyc&quot;
guillaume@ubuntu:~/0x02$ ./4-hidden_discovery.py | sort
my_secret_santa
print_hidden
print_school
guillaume@ubuntu:~/0x02$ 
</code></pre>

</div>

<div class="list-group">
<!-- Task URLs -->

<!-- Github information -->
<div class="list-group-item">
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>alx-higher_level_programming</code></li>
<li>Directory: <code>0x02-python-import_modules</code></li>
<li>File: <code>4-hidden_discovery.py</code></li>
</ul>
</div>

<!-- Self-paced manual review -->
</div>

<!-- Panel footer - Controls -->
<div class="panel-footer">
<div class="align-items-center d-flex justify-content-between">

<div>
<button class="student_task_done btn btn-default btn-sm no" data-task-id="1087">
<span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
<span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
<span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
Done<span class="no pending">?</span><span class="yes">!</span>
</button>

<button class="student-task-done-by btn btn-default btn-sm" data-task-id="1087" data-batch-id="26" data-toggle="modal" data-target="#task-1087-users-done-modal">
Help
</button>
<div class="modal fade users-done-modal" id="task-1087-users-done-modal" data-task-id="1087" data-batch-id="26">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Students who are done with "4. Who are you?"</h4>
</div>
<div class="modal-body">
<div class="list-group">
</div>
<div class="spinner">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
</div>
</div>
</div>
</div>


<button class="btn btn-default btn-sm check-your-task-1087-modal-button" data-task-id="1087" data-toggle="modal" data-target="#task-test-correction-1087-correction-modal" id="task-num-4-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1087}'>
Check your code
</button>
<div class="modal fade task_correction_modal student_modal" id="task-test-correction-1087-correction-modal">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Correction of "4. Who are you?"</h4>
</div>
<div class="modal-body">
<div class="actions">
<center>
<div class="alert alert-info hidden"></div>

<button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1087">Start a new test</button>
<button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

<div class="spinner" style="display: none;">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
<div class="info"></div>
</center>
</div>
<div class="result"></div>

<div class="help">
<button data-task-id="1087">
<i aria-hidden="true" class="fa fa-info-circle "></i>
</button>
<div class="help-container" data-task-id="1087">
<div class="check-line">
<div class="check-inline requirement success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Requirement success
</div>
<div class="check-inline requirement fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Requirement fail
</div>
</div>
<div class="check-line">
<div class="check-inline code success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Code success
</div>
<div class="check-inline code fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Code fail
</div>
</div>
<div class="check-line">
<div class="check-inline efficiency success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Efficiency success
</div>
<div class="check-inline efficiency fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Efficiency fail
</div>
</div>
<div class="check-line">
<div class="check-inline answer success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Text answer success
</div>
<div class="check-inline answer fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Text answer fail
</div>
</div>
<div class="check-line">
<div class="check-inline requirement fail offline">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Skipped - Previous check failed
</div>
</div>
</div>
</div>

</div>
</div>
</div>
</div>



<button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1087}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

<button class="btn btn-default btn-sm" data-task-id="1087" data-toggle="modal" data-target="#task-qa-review-1087-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1087}'>
QA Review
</button>
<div class="modal fade task_get_qa_review" id="task-qa-review-1087-modal" data-correction-id="12737951" data-task-id="1087">
<div class="modal-dialog modal-lg">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">4. Who are you?</h4>
</div>
<div class="modal-body">
<div class="spinner gap">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="review-container">
<div class="review-corrector"></div>
<div class="review-github well" style="display:none">
<h5>Commit used:</h5>
<ul>
<li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
<li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
<li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
<li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
<li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
<li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
</ul>
</div>
<div class="review-percentage_down"></div>
<ul class="review-checks list-group sm-gap"></ul>
<div class="review-comment"></div>
</div>
</div>
</div>
</div>
</div>

</div>


<div class="fs-4">
</div>
</div>


</div>
</div>

</div>
<div data-role="task1090" data-position="6" id="task-num-5">
<div class="panel panel-default task-card " id="task-1090">
<span id="user_id" data-id="197885"></span>

<div class="panel-heading panel-heading-actions">
<h3 class="panel-title">
5. Everything can be imported
</h3>

<div>
<span class="label label-info">
mandatory
</span>
</div>
</div>

<div class="panel-body">
<span id="user_id" data-id="197885"></span>

<!-- Progress vs Score -->
<div class="task_progress_score_bar" data-task-id="1090" data-correction-id="12737951">
<div class="task_progress_bar" style="width: 0.0%">
<div class="task_score_bar" style="width: NaN%">
</div>
</div>
<div class="task_progress_score_text">
Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
</div>
</div>

<!-- Task Body -->
<p>Write a program that imports the variable <code>a</code> from the file <code>variable_load_5.py</code> and prints its value.</p>

<ul>
<li>You are not allowed to use <code>*</code> for importing or <code>__import__</code></li>
<li>Your code should not be executed when imported</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x02$ cat variable_load_5.py
#!/usr/bin/python3
a = 98
&quot;&quot;&quot;Simple variable
&quot;&quot;&quot;

guillaume@ubuntu:~/0x02$ ./5-variable_load.py
98
guillaume@ubuntu:~/0x02$
</code></pre>

</div>

<div class="list-group">
<!-- Task URLs -->

<!-- Github information -->
<div class="list-group-item">
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>alx-higher_level_programming</code></li>
<li>Directory: <code>0x02-python-import_modules</code></li>
<li>File: <code>5-variable_load.py</code></li>
</ul>
</div>

<!-- Self-paced manual review -->
</div>

<!-- Panel footer - Controls -->
<div class="panel-footer">
<div class="align-items-center d-flex justify-content-between">

<div>
<button class="student_task_done btn btn-default btn-sm no" data-task-id="1090">
<span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
<span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
<span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
Done<span class="no pending">?</span><span class="yes">!</span>
</button>

<button class="student-task-done-by btn btn-default btn-sm" data-task-id="1090" data-batch-id="26" data-toggle="modal" data-target="#task-1090-users-done-modal">
Help
</button>
<div class="modal fade users-done-modal" id="task-1090-users-done-modal" data-task-id="1090" data-batch-id="26">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Students who are done with "5. Everything can be imported"</h4>
</div>
<div class="modal-body">
<div class="list-group">
</div>
<div class="spinner">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
</div>
</div>
</div>
</div>


<button class="btn btn-default btn-sm check-your-task-1090-modal-button" data-task-id="1090" data-toggle="modal" data-target="#task-test-correction-1090-correction-modal" id="task-num-5-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1090}'>
Check your code
</button>
<div class="modal fade task_correction_modal student_modal" id="task-test-correction-1090-correction-modal">
<div class="modal-dialog">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Correction of "5. Everything can be imported"</h4>
</div>
<div class="modal-body">
<div class="actions">
<center>
<div class="alert alert-info hidden"></div>

<button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1090">Start a new test</button>
<button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

<div class="spinner" style="display: none;">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="error"></div>
<div class="info"></div>
</center>
</div>
<div class="result"></div>

<div class="help">
<button data-task-id="1090">
<i aria-hidden="true" class="fa fa-info-circle "></i>
</button>
<div class="help-container" data-task-id="1090">
<div class="check-line">
<div class="check-inline requirement success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Requirement success
</div>
<div class="check-inline requirement fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Requirement fail
</div>
</div>
<div class="check-line">
<div class="check-inline code success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Code success
</div>
<div class="check-inline code fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Code fail
</div>
</div>
<div class="check-line">
<div class="check-inline efficiency success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Efficiency success
</div>
<div class="check-inline efficiency fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Efficiency fail
</div>
</div>
<div class="check-line">
<div class="check-inline answer success">
<i aria-hidden="true" class="fa fa-check-circle "></i>
Text answer success
</div>
<div class="check-inline answer fail">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Text answer fail
</div>
</div>
<div class="check-line">
<div class="check-inline requirement fail offline">
<i aria-hidden="true" class="fa fa-times-circle "></i>
Skipped - Previous check failed
</div>
</div>
</div>
</div>

</div>
</div>
</div>
</div>



<button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1090}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

<button class="btn btn-default btn-sm" data-task-id="1090" data-toggle="modal" data-target="#task-qa-review-1090-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1090}'>
QA Review
</button>
<div class="modal fade task_get_qa_review" id="task-qa-review-1090-modal" data-correction-id="12737951" data-task-id="1090">
<div class="modal-dialog modal-lg">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">5. Everything can be imported</h4>
</div>
<div class="modal-body">
<div class="spinner gap">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div class="review-container">
<div class="review-corrector"></div>
<div class="review-github well" style="display:none">
<h5>Commit used:</h5>
<ul>
<li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
<li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
<li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
<li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
<li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
<li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
</ul>
</div>
<div class="review-percentage_down"></div>
<ul class="review-checks list-group sm-gap"></ul>
<div class="review-comment"></div>
</div>
</div>
</div>
</div>
</div>

</div>


<div class="fs-4">
</div>
</div>


</div>
</div>

</div>

<p class="lg-gap">
<form class="button_to" method="post" action="/projects/239/unlock_optionals"><input id="unlock_optional_btn" class="btn btn-primary btn-block" data-confirm="Are you sure? Make sure you focused on the mandatory tasks first" data-disable-with="Unlocking 4 advanced tasks..." data-gtm-custom-event-name="project_unlock_advanced_tasks" type="submit" value="Done with the mandatory tasks? Unlock 4 advanced tasks now!" /><input type="hidden" name="authenticity_token" value="9I7WqI0m8dmQeP0Y0RKaBsBmob0NlxmfnjRetsPmaUjApidV0lqpetq9tcbPcE9vjdUdgReeWMmR__JIXKoRhQ" autocomplete="off" /></form>
</p>




<div class="modal fade" id="container-specs-modal"><div class="modal-dialog modal-lg"><div class="modal-content"><div class="modal-header"><button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button><h4 class="modal-title">Recommended Sandbox</h4></div><div class="modal-body"><div data-react-class="user_containers/ContainerSpecs" data-react-props="{&quot;containerModelName&quot;:&quot;Sandbox&quot;,&quot;containerSpecs&quot;:[{&quot;description&quot;:&quot;\u003cp\u003eBasic Ubuntu 20.04, with vim, emacs, curl, wget and all needed for Foundations\u003c/p\u003e\n&quot;,&quot;id&quot;:39,&quot;name&quot;:&quot;Ubuntu 20.04&quot;,&quot;online&quot;:true,&quot;container&quot;:{&quot;container_id&quot;:null,&quot;id&quot;:239271,&quot;restart_uri&quot;:&quot;/user_containers/239271/restart.json&quot;,&quot;status&quot;:&quot;asleep&quot;,&quot;uri&quot;:&quot;/user_containers/239271.json&quot;,&quot;wake_uri&quot;:&quot;/user_containers/239271/wake.json&quot;,&quot;webterm_uri&quot;:&quot;/user_containers/239271/webterm&quot;,&quot;host&quot;:null,&quot;password&quot;:&quot;2deaf74c415af9350d02&quot;,&quot;ports&quot;:{&quot;22&quot;:33287,&quot;3000&quot;:33284,&quot;443&quot;:33285,&quot;5001&quot;:33280,&quot;80&quot;:33286,&quot;8080&quot;:33278,&quot;3306&quot;:33283,&quot;4000&quot;:33282,&quot;5000&quot;:33281,&quot;8000&quot;:33279}}}],&quot;containersLimit&quot;:2,&quot;csrfToken&quot;:&quot;LDBeuxQf5cRiSw3aB6Rg4-iDgE81swjm7Iu_BlkEOcNxrsxoD5dMH8TbIsA9DTVzGftue_7Vmdeu-s6hh24GcA&quot;,&quot;startStatusURI&quot;:&quot;/user_containers/start_status.json&quot;,&quot;startURI&quot;:&quot;/user_containers/start.json&quot;}" data-react-cache-id="user_containers/ContainerSpecs-0"></div></div></div></div></div>

</div>
</div>


</article>

<div class="copyright">Copyright ?? 2023 ALX, All rights reserved.</div>

</main>

<button class="btn btn-primary" id="search-button" data-search-active="false" data-toggle="modal" data-target="#search-modal">
<i aria-hidden="true" class="fa fa-search "></i>
<i aria-hidden="true" class="fa fa-window-minimize "></i>
</button>

<div class="modal fade" id="search-modal" tabindex="-1" role="dialog" aria-labelledby="search-modal-label">
<div class="modal-dialog modal-md">
<div class="modal-content">
<div class="modal-header">
<div id="search-bar-container">
<input id="search-bar"
type="text"
name="hbtn-search-bar"
placeholder="???Start search by typing in this field???">
</div>

</div>
<div class="modal-body">
<div id="modal-spinner" class="spinner gap">
<div class="bounce1"></div>
<div class="bounce2"></div>
<div class="bounce3"></div>
</div>
<div id="search-results-container">
</div>

</div>
</div>
</div>
</div>



<div class="modal fade" id="markdownGuideModal" tabindex="-1" role="dialog" aria-labelledby="markdownGuideModalLabel" aria-hidden="true">
<div class="modal-dialog modal-md">
<div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<h4 class="modal-title">Markdown Guide</h4>
</div>
<div class="modal-body">
<h4>Emphasis</h4>
<pre>**<strong>bold</strong>**
*<em>italics</em>*
~~<strike>strikethrough</strike>~~</pre>
<h4>Headers</h4>
<pre># Big header
## Medium header
### Small header
#### Tiny header</pre>
<h4>Lists</h4>
<pre>* Generic list item
* Generic list item
* Generic list item

1. Numbered list item
2. Numbered list item
3. Numbered list item</pre>
<h4>Links</h4>
<pre>[Text to display](http://www.example.com)</pre>
<h4>Quotes</h4>
<pre>> This is a quote.
> It can span multiple lines!</pre>
<h4>Images</h4>
<p>CSS style available: <code>width, height, opacity</code></p>
<pre>![](http://www.example.com/image.jpg)
![](http://www.example.com/image.jpg | width: 200px)
![](http://www.example.com/image.jpg | height: 124px | width: 80px | opacity: 0.6)
</pre>
<h4>Tables</h4>
<pre>| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| John     | Doe      | Male     |
| Mary     | Smith    | Female   |

<em>Or without aligning the columns...</em>

| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| John | Doe | Male |
| Mary | Smith | Female |
</pre>
<h4>Displaying code</h4>
<pre>`var example = "hello!";`

<em>Or spanning multiple lines...</em>

```
var example = "hello!";
alert(example);
```</pre>
</div>
</div>
</div>
</div>


</body>
</html>
