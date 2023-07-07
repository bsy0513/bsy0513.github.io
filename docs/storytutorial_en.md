---
layout: page
title: T4Framework
subtitle: Story Tutorials with T4Framework
---
<style>
    .embed-container {
        position: relative;
        padding-bottom: 56.25%;
        height: 0;
        overflow: hidden;
        max-width: 100%;
    }

    .embed-container iframe, .embed-container object, .embed-container embed {
        position: absolute;
		top: 1%;
		down: 1%;
        left: 0%;
        width: 100%;
        height: 100%;
    }
</style>

<hr/>
Have you ever thought about creating your own content? Today, people communicate with others by posting their writings, pictures, or videos on various online platforms such as Blog, Instagram, YouTube, etc. Such a method is a form of one-way communication in which only creators can affect users. With T4Framework, however, you can easily create a virtual space where you can exhibit videos and arts, or the whole space may  serve as a story-telling complex. Invite people over to your virtual world to let them explore and experience your story! This way, T4Framework supports two-way communication between creators and users.
<br/>

A framework based on Unreal Engine, T4Framework makes it possible to create 3D content without coding or scripting. The Story Tutorial project that's introduced below was developed solely with T4Framework and some free assets.
<br/>
<br/>
<hr/>
<center><h3>- What is The Story Tutorial? -</h3></center>

The Story Tutorial is a simple content into which people can enter and experience its narrative firsthand. A player can easily control a character to follow the plot of the content and watch the videos that the creator placed in it. Here, we plan to introduce how the Story Tutorial was made with T4Framework.<br/>

*Please check the Story Tutorial Documents if you want more detailed information.*<br/>
<br/>
<hr/>
<center><h3>- The Story Tutorial Playthrough -</h3></center>

<div class="embed-container"><iframe src="https://youtube.com/embed/lJO0kJMfQDU" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ StoryTutorial Metahuman Ada ver. ]</h4></center>

The Story Tutorial is a story about a woman named Ada, who explores a mysterious cave. In the cave, she meets a robot who has been eagerly looking for something. Eventually, she manages to find what it was looking for, and as a result a TV in the cave displays a video, after which the Story Tutorial ends. Let's check how each entity (Player, Robot, Box, etc.), narrative, and scene directing were developed with T4Framework.<br/>
<br/>
<br/>
<hr/>
<center><h3>- The Story Tutorial's Core Elements -</h3></center>

Let us introduce the core elements of the Story Tutorial. It consists of the main character (Player), Robot (NPC), backgrounds (Map), box (Goods), TV (Prop), and Zone. Each of the listed element could be created and set up with the help of T4Framework and some free assets.<br/><br/>


<h4> 1) The Main Character (Player) </h4>

<table border=0 width="100%" height="540">
	<tr>
		<td><center><img src="https://user-images.githubusercontent.com/101547387/178220413-1ff38c5e-a66f-40e2-8cd2-f7b936f092e7.png" width="360" height="500"></center></td>
    </tr>
</table>

This is the protagonist of the Story Tutorial, Ada.<br/>
Ada is a character created by utilizing metahuman resources provided by Unreal Engine.<br/>
More information about metahumans can be found at the link below.<br/>
Reference: <a href="https://docs.metahuman.unrealengine.com/en-US/" target="_blank">Metahuman Creator </a><br/>

<img src="https://user-images.githubusercontent.com/101547387/178220974-63105a0c-e8d7-4a01-8ed8-fca282bac804.png">

This is T4Framework's Entity Editor. You can create and edit various assets here. 
You can set the main character's appearance via T4CharacterEntity asset.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/_t-jHHvjULQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Character Entity Video ]</h4></center>

By utilizing the State Layer feature, some basic animations for the character have been added. You can check the character's motion in the Viewport at the center of your screen.<br/><br/>

<h4> 2) The Robot (NPC) </h4>

<table border=0 width="100%" height="420">
	<tr>
		<td><center><img src="https://user-images.githubusercontent.com/101547387/178221270-2200eb2f-4424-482a-b811-9bdf5e883ec2.png" width="308" height="384"></center></td>
    </tr>
</table>

This is the robot, another character featured in the Story Tutorial. The robot is classified as a non-player character (NPC) because players cannot control it. It goes by 'omE' and features as the main character/player in Gryun's project.<br/><br/>
Reference: <a href="https://t4framework.com/GryunKim/" target="_blank">Gryun Kim with T4Framework </a><br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/ddUf4FG5fSQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ omE Skill Layer Video ]</h4></center>

The Skill Layer feature was used to add various animations that a character may perform based on the situation it's currently in. In the Story Tutorial, a reactionary animation was added to Robot so it can act accordingly after receiving the box from the protagonist.<br/><br/>


<h4> 3) Backgrounds (Map) </h4>

<img src="https://user-images.githubusercontent.com/101547387/178221748-be40f025-1bc2-431d-9325-d146e62f6c31.png"><br/>

This is "Cave Entrance," the very first map that a player enters into when playing through the Story Tutorial. It's a cave with exits on both sides.<br/>

<img src="https://user-images.githubusercontent.com/101547387/178221759-230fe6df-beee-4230-a244-076c1c730a85.png"><br/>

Junkyard is the second map of the Story Tutorial. There's only a single road a player can follow, at the end of which exist a place where various scrap metals can be looted.
The Maps featured in the Story Tutorial were created with the T4MapEntity feature.<br/><br/>

<h4> 4) The Box (Goods) </h4>

<table border=0 width="100%" height="540">
	<tr>
		<td><center><img src="https://user-images.githubusercontent.com/101547387/178224950-051699fe-9da1-4650-a937-ca50b940c30d.png"></center></td>
    </tr>
</table>

This is the box that was placed next to the robot.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/o4ARppP_krY" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Goods Entity Video ]</h4></center>

The box was created with the T4GoodEntity feature, and its size was adjusted so it's neither too big nor small compared to the main character.<br/><br/>


<h4> 5) TV (Prop) </h4>

<img src="https://user-images.githubusercontent.com/101547387/178226822-49641aba-87c7-423d-a602-be5b4227fe67.png"><br/>

This is the TV that Robot turned on after taking the box.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/M3jU9zdYAAk" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Prop Entity Video ]</h4></center>

Using the T4PropEntity feature, you can combine Media Screen and Hull Frame to create a TV prop. In addition, a video clip was set up to be played on the TV screen as Ada the protagonist approaches it.<br/><br/>


<h4> 6) Zone </h4>

<img src="https://user-images.githubusercontent.com/101547387/178227078-32ab4985-bd0d-4c50-bd63-e1c005621dca.png"><br/>

Although it wasn't shown in the Story Tutorial playthrough, there were two Zones installed at both entrances to the cave to invoke certain events within the content. A Zone is a kind of Entity that acts as an event trigger. When Ada the protagonist enters a Zone, she gets forced to choose one of the two options shown in a message box, which asks if she's willing to follow the road or just stay inside the cave to explore it a bit more. You can create Zones in any shape you want via the T4ZoneEntity feature.<br/>

<img src="https://user-images.githubusercontent.com/101547387/175938532-c262cb19-4779-4d89-9a92-af2346f36faf.png"><br/>

As for a Prop, you can specify its corresponding Zone directly in the Entity Editor. In the Story Tutorial, a video clip is set to be played on the TV as the player enters the area.<br/><br/>
<br/>
<br/>
<hr/>
<center><h3>- The Story Tutorial Project -</h3></center>

All the assets needed for the Story Tutorial have thus been created. Now it's necessary to properly position these assets within a Map. T4Framework automatically forms databases (DB) of the assets by creating a project and incorporating each asset into it. You can easily develop a story content by adding appropriate assets for each category and dragging them to your desired location in a Map. As the DBs for assets get created automatically as those assets get registered to your project, no additional coding work is required.<br/>

The Quest Flows that make up the Story Tutorial are described below.<br/><br/>

<h4> 1) Cave Entrance Settings </h4>

<img src="https://user-images.githubusercontent.com/101547387/178391916-bf0402fd-7719-4e3c-90aa-6687b46fbce5.png"><br/>

In the Content Editor, you can create a project in which to place assets and set up various content-related events to be triggered. When you're done developing your content, you can export the final version of your project into an executable package.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/jBsq2vRFCUQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ CaveEntrance Setting Video ]</h4></center>

In the Content Editor, the player's starting locaiton and some quest-triggering Zones' positions were set up.<br/><br/>

<h4> 2) Junkyard Settings </h4>

<img src="https://user-images.githubusercontent.com/101547387/178395243-c7f00b93-1170-4cc6-b9bf-59ea59cbbf60.png"><br/>

Placed in the Junkyard Map are objects such as omE, box, and TV.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/j1173DvSvWw" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ omE and Waypoint Setting Video ]</h4></center>

On top of setting omE's location, its Waypoints were also set.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/VwP4_ODNwGQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><b>[ Box and TV Setting Video ]</b></center>
The box and TV were placed in the right place also.<br/><br/>
<br/>
<br/>
<hr/>
<center><h3>- The Story Tutorial Narrative (Quest) -</h3></center>

The Story Tutorial's narrative consists of Ada entering Cave Entrance and then stumbling upon the robot in the Junkyard area. With the Quest Flow feature of T4Framework, developers could easily set up various aspects of the project such as when characters and items should appear, at what timing dialogues should pop up, and when a video clip should be played. Unlike other game engines that require coding and scripting, in T4Framework one can easily create quests by simply configuring quest nodes that perform desired functions that include, but are not limited to, progressing inter-character conversations, and inducing players to act in certain ways.<br/>

What's described below is a more detailed explanation on the Story Tutorial's Quest Flow composition.<br/><br/>

<hr/>
<h4> 1) Cave Entrance </h4>
<h5> Opening (Timelines 00:00~00:07) </h5>

<img src="https://user-images.githubusercontent.com/101547387/179718687-587ed824-56ba-4b66-8d40-3e679f1d72e8.png"><br/>

This is the Quest Flow that dictates the beginning part of the Story Tutorial. You can see that the quest is composed of various nodes. Nodes have been set up in a way that turns the lights on as Ada the protagonist enters the cave for the first time, right after which the camera shows around the cave that's lighted up. Afterward, Ada gets forced to make a choice on which way to choose, in the process of which her self-talking dialogue of "I see two different paths ahead. Which one should I choose?" pops up. She was also set up to perform an animation that makes her head alternate between the two different paths.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/OiGAbmHYAck" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Opening QuestFlow Video ]</h4></center>

Narratives were created with the T4QuestFlow feature. One can simply drag and drop Quest nodes to set up the sequence of narratives and determine what kinds of directing techniques or functions will be added into it.<br/><br/>

<h5> Left Exit & Right Exit (Timelines 00:11~00:27) </h5>

<img src="https://user-images.githubusercontent.com/101547387/179718796-799bf523-d131-49a6-b33a-f6c492fe6daf.png"><br/>

When you arrive at either the left or right paths of the cave, you get to choose whether to follow a path or look around the cave a bit more. If you choose to walk along the path, the quest ends and you move on to Junkyard. If you instead choose the option to look around the cave, the quest will be aborted.<br/>

<img src="https://user-images.githubusercontent.com/101547387/179736045-63cbc53c-6779-4883-aa32-ceb00271c2ae.png" width="100%" height="540">
<img src="https://user-images.githubusercontent.com/101547387/179718874-c61afe50-74e5-4c6b-af99-30d150965054.png"><br/>

By using the Branch function, you can make your quest lead to different results based on a player's choice. With Quest Flow, you can set up what dialogues should pop up or what intermission scenes should be displayed for each possible path a player can may when progressing through a quest.<br/><br/>

<h4> 2) Junkyard </h4>
<h5> Encountering the robot (Timelines 00:30~01:05) </h5>

<img src="https://user-images.githubusercontent.com/101547387/179718966-78568249-44bd-4629-994f-52cb6ff0b6c9.png"><br/>

Ada selects one of the paths on either side of the cave, walking along which she eventually reaches the Junkyard area. Here Ada stumbles upon a robot(omE) who's looking for a missing box. After she hands the box to the robot, it moves to the front of the TV with the box in its hands.<br/>

<table border=0 width="100%" height="370">
	<tr>
		<td>
<center><img src="https://user-images.githubusercontent.com/101547387/179719138-3cdf5685-5a10-47e0-be96-ac5810c3a5d4.png"></center></td>
    </tr>
</table>		

This Quest was configured to proceed to the next step only when the player owns the required item. The HasItems node checks whether the player has the item and, if he does, the flow of the quest will proceed to the subsequent Interaction node. As soon as Robot retrieves the box that Ada found, a dialogue will take place.<br/>

<img src="https://user-images.githubusercontent.com/101547387/175945429-bf1b9f9e-5f38-47d6-8eeb-fb4f26c3a840.png"><br/>

An Action node was configured so as to make omE move to its destination when it receives the box. In order to emphasize its movement, the player becomes immobile during the transitory scene, and the camera was set to track omE's walking path.<br/><br/>

<h5> The Ending (Timelines 01:11~01:17) </h5>

<img src="https://user-images.githubusercontent.com/101547387/179719233-cc6600d9-9d42-4ac4-a4f3-642464880540.png"><br/>

Once omE reaches its destination, Ada sets about following the robot. As she approaches the TV in front of the robot, a video clip gets played on the TV screen and that same video (the ending clip) will be enlarged to take up your whole monitor screen and be played until its end.<br/><br/>
<br/>
<br/>
<hr/>
<center><h3>- Story Tutorial Direction -</h3></center>

This section introduces the directing techniques and visual effects used in the Story Tutorial. The visual effect that made the box--which Robot was looking for--shine was made with T4's Action Pack feature. Likewise, the camerawork that showed the left and right side of the Cave Entrance and tracked the robot's movement as it walked towards the TV could be achieved with T4's Camera Walk feature. Lastly, T4's UI feature was used to implement the effect of the video clip on TV getting bigger to eventually take up the entire monitor screen as the content ends.<br/>

The description below addresses how T4's directing tools (Action Pack, Camera Walk, and End Direction (UI)) can be utilized in your project.<br/><br/>

<h4> 1) Action Pack </h4>

<img src="https://user-images.githubusercontent.com/101547387/178400444-49324593-9dd4-4fd0-ba03-1a8cee2ed0be.png"><br/>

This is the box that was placed in Junkyard. An Action Pack was added to it to make it glow.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/WNQV11MkvEI" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Action Pack Video ]</h4></center>

This glowing Action was added to the box to make it easier for a player to find the box, which is placed next to omE. With T4Framework's Action Pack, you can easily produce such visual effects.

<br/><br/>

<h4> 2) Camera Walk </h4>

<img src="https://user-images.githubusercontent.com/101547387/178402405-04ff8b5e-1148-4206-9374-f5d7398e3c2d.png"><br/>

A camera can be made to track a character's movement, which in our case happened to be omE the robot. The mannequin at the center is marking omE's current position. You can preview how it will actually look within a scene in the viewport at the bottom-left corner of the screen; the camera will move along the white line.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/S_b-dCgCefE" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Camera Walk Setting Video ]</h4></center>

You can add a Camera in the Content Editor to set up your desired Camera Walk.<br/><br/>

<h4> 3) Ending Direction (UI) </h4>

<table border=0 width="100%" height="370">
	
<img src="https://user-images.githubusercontent.com/101547387/179735477-95f7d3ec-3a7a-4a92-83bf-90e13d14d4b2.png"><br/><br/>

When the Story Tutorial ends, the video clip that was being played on the TV will get bigger and bigger to eventually take up the whole monitor screen, which serves as an ending screen for the tutorial.<br/><br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/B1K_l3vE3FQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Ending UI Setting Video ]</h4></center>

After registering a video clip of your choice as a UI in the Content Editor, you can easily set when and how the ending scene should take place via the QuestFlow feature (take a look at the Junkyard quest for your reference).<br/><br/>
<br/>
<hr/>
<center><h3>- End of the Story Tutorial -</h3></center>

Traditionally, the creation of 3D content has required a deep understanding of Unreal Engine and coding, but with T4Framework even non-experts can develop 3D content easily and quick. The Story Tutorial introduced here is just one example of what you can achieve with T4Framework; with your infinite creativity, you can develop more diverse and high-quality content with the help of T4.<br/>

T4Framework will always be here to help you create great 3D content. 
Thank you.<br><br><br><br/>

<center><a href="https://github.com/VirtualFlowInc/VirtualFlowStudio_Public/">> <b>Free Evaluation</b> <</a><br><br></center>
<center><a href="https://t4framework.com/storytutorial/"><b>Korean</b></a> &nbsp;/&nbsp; <a href="https://t4framework.com/index_en/"><b>HOME</b></a></center>
