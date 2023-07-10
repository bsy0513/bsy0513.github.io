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
나만의 콘텐츠를 만들어보고 싶다는 생각을 해보신 적이 있으신가요? 많은사람들이 글, 그림, 또는 영상 등을 온라인에 게시하고 사람들과 소통하고자합니다. 이러한 방식은 화자가 청자에게 이야기를 들려주는, 일방향적 소통을추구합니다. 그러나 T4Framework은 공간을 창조하고, 그 안에 청자를 초대하여 자유롭게 공간을 탐험하며 이야기를 체험하고 느끼는 것을 가능하게 합니다. T4Framework을 사용하면 전시관처럼 가상 공간 안에서 다양한 영상이나 그림 등을 전시하거나,공간 전체가 하나의 이야기가 되어 청자와 양방향적 소통을하는 것 모두 쉽게 구현할 수 있습니다.
<br/>

언리얼 엔진을 사용하는 T4Framework은 코딩과 스크립트 작업 없이 3D콘텐츠를 제작할 수 있도록 도와줍니다. 아래 소개해드릴 스토리 튜토리얼(Story Tutorial)은 무료 에셋과 T4Framework을 사용하여 제작한 3D 콘텐츠 입니다.
<br/>
<br/>
<hr/>
<center><h3>- 스토리 튜토리얼이란? -</h3></center>

스토리 튜토리얼은 청자가 직접 공간 안으로 들어와 이야기를 체험해 나가는 방식을 가볍게 보여드리는 콘텐츠입니다. 플레이어는 자유롭게 조작하며 이야기의 흐름을 따라가고, 화자가 준비한 미디어를 감상할 수 있습니다. 여기서는 T4Framework을 사용하여 스토리 튜토리얼이 어떻게 제작되었는지에 대해 소개해드리고자 합니다.<br/>

*자세한 제작기는 튜토리얼 문서를 참고해주시기 바랍니다.*<br/>
<br/>
<hr/>
<center><h3>- 스토리 튜토리얼 플레이 영상 -</h3></center>


<div class="embed-container"><iframe src="https://youtube.com/embed/Jt9bD31YzNE" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ 스토리튜토리얼 Metahuman Ada ver. ]</h4></center>

스토리 튜토리얼은 주인공 Ada가 동굴 안을 탐험하는 짧은 이야기입니다. 동굴을 탐험하다 무언가를 찾고 있는 로봇을 만나고, 로봇이 찾던 상자를 건네주자 동굴 안에 있던 TV에서 영상이 켜지며 콘텐츠는 종료됩니다. 각각의 등장요소(주인공, 로봇, 상자 등), 내러티브 그리고 연출이 T4Framework을 사용해 어떻게 제작되었는지 살펴보겠습니다.
<br/>
<br/>
<hr/>
<center><h3>- 스토리 튜토리얼 등장요소 -</h3></center>

스토리 튜토리얼의 등장요소들을 소개합니다. <b>주인공, 로봇(NPC), 배경(맵), 상자(굿즈), TV(프랍)</b> 그리고 <b>존(Zone)</b>에 대해 설명드리겠습니다. 각 요소들은 무료 에셋과 T4Framework을 사용하여 제작되었습니다.<br/><br/>


<h4> 1) 주인공 (Player) </h4>

<table border=0 width="100%" height="540">
	<tr>
		<td><center><img src="https://user-images.githubusercontent.com/101547387/178220413-1ff38c5e-a66f-40e2-8cd2-f7b936f092e7.png" width="360" height="500"></center></td>
    </tr>
</table>

스토리 튜토리얼의 주인공 Ada입니다. Ada는 언리얼 엔진에서 제공하는 메타휴먼 크리에이터에서 제작된 캐릭터입니다.<br>
메타휴먼에 대한 자세한 내용은 아래 링크에서 확인해볼 수 있습니다.<br><br>
참고: <a href="https://docs.metahuman.unrealengine.com/en-US/" target="_blank">언리얼 엔진: 메타휴먼 </a><br/>

<img src="https://user-images.githubusercontent.com/101547387/178220974-63105a0c-e8d7-4a01-8ed8-fca282bac804.png">

T4Framework의 Entity 편집 페이지입니다. 이곳에서 각종 에셋들을 만들고 편집할 수 있습니다.
주인공 캐릭터를 만들기 위해 T4CharacterEntity을 열어 캐릭터의 외형을 설정하였습니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/_t-jHHvjULQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Character Entity 영상 ]</h4></center>

State Layer 기능을 사용하여 캐릭터의 기본 애니메이션을 추가하였습니다. 가운데 Viewport 화면에서 캐릭터의 모션을 확인할 수 있습니다.<br/><br/>

<h4> 2) 로봇(NPC) </h4>

<table border=0 width="100%" height="420">
	<tr>
		<td><center><img src="https://user-images.githubusercontent.com/101547387/178221270-2200eb2f-4424-482a-b811-9bdf5e883ec2.png" width="308" height="384"></center></td>
    </tr>
</table>

스토리 튜토리얼의 또다른 등장인물인 로봇입니다. 이 로봇은 플레이어가 직접 조작하는 캐릭터가 아니기 때문에 Non Player Character(NPC)로 분류됩니다. 이 로봇의 명칭은 omE이며, 그륜님 프로젝트에서는 주인공/플레이어로 설정되어있습니다.<br/><br/>
참고: <a href="https://t4framework.com/GryunKim_ko/" target="_blank">Gryun Kim with T4Framework </a><br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/ddUf4FG5fSQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ omE Skill Layer 추가 영상 ]</h4></center>

Skill Layer 기능을 시용하여 캐릭터에게 상황에 적절한 애니메이션을 추가하였습니다. 스토리 튜토리얼에서는 처음 로봇이 상자를 찾을 때, 그리고 주인공에게서 상자를 건네받은 후를 위한 애니메이션을 추가하였습니다.<br/><br/>


<h4> 3) 배경 (Map) </h4>

<img src="https://user-images.githubusercontent.com/101547387/178221748-be40f025-1bc2-431d-9325-d146e62f6c31.png"><br/>

스토리 튜토리얼의 첫번째 맵인 <b>Cave Entrance</b> 입니다. 양 옆에 출구가 있는 동굴입니다.<br/>

<img src="https://user-images.githubusercontent.com/101547387/178221759-230fe6df-beee-4230-a244-076c1c730a85.png"><br/>

스토리 튜토리얼의 두번째 맵인 <b>Junkyard</b> 입니다. 길은 하나이며 길을 따라가면 여러 고철이 모여있는 장소가 나옵니다.
스토리 튜토리얼이 진행되는 맵들은 T4MapEntity 기능을 사용하여 제작하였습니다.<br/><br/>

<h4> 4) 상자 (Goods) </h4>

<table border=0 width="100%" height="540">
	<tr>
		<td><center><img src="https://user-images.githubusercontent.com/101547387/178224950-051699fe-9da1-4650-a937-ca50b940c30d.png">
</center></td>
    </tr>
</table>

로봇 우측에 배치되어 있던 상자입니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/o4ARppP_krY" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Goods Entity 제작 영상 ]</h4></center>

T4GoodsEntity 기능을 사용하여 상자를 제작한 후, 주인공 캐릭터와 크기를 비교하며 조정해 주었습니다.<br/><br/>


<h4> 5) TV (Prop) </h4>

<img src="https://user-images.githubusercontent.com/101547387/178226822-49641aba-87c7-423d-a602-be5b4227fe67.png"><br/>

스토리 튜토리얼에서 로봇이 상자를 가져가서 영상을 켠 TV입니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/M3jU9zdYAAk" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Prop Entity 제작 영상 ]</h4></center>

T4PropEntity 기능을 사용하여 Media Screen과 Hull Frame을 조합하여 TV 프랍을 제작했습니다. 또한 만들어진 TV의 화면 부분에 영상을 추가하여 주인공 Pia가 다가갈 때 영상이 켜지도록 설정하였습니다.<br/><br/>


<h4> 6) 존 (Zone) </h4>

<img src="https://user-images.githubusercontent.com/101547387/178227078-32ab4985-bd0d-4c50-bd63-e1c005621dca.png"><br/>

스토리 튜토리얼 플레이 영상에서는 나타나지 않았지만, 이벤트를 발동시키기 위해 동굴 양쪽 입구에는 존(Zone)이 설치되어 있었습니다. 이벤트 트리거 역할을 하는 존(Zone)은 Entity의 한 종류입니다. 주인공 Pia가 해당 존 안으로 들어가면 길을 따라 들어갈지, 아니면 동굴을 더 탐색할 지를 묻는 선택지가 등장하도록 설정되어 있었습니다. T4ZoneEntity 기능을 사용하여 원하는 모양의 존을 제작할 수 있습니다.<br/>

<img src="https://user-images.githubusercontent.com/101547387/175938532-c262cb19-4779-4d89-9a92-af2346f36faf.png"><br/>

참고로 프랍의 경우, Entity 설정에서 직접 존을 지정해줄 수 있습니다. 스토리 튜토리얼에서는 해당 영역 안으로 플레이어가 들어올 시 TV 속 영상이 켜지도록 설정하였습니다.
<br/>
<br/>
<hr/>
<center><h3>- 스토리 튜토리얼 프로젝트 (Project) -</h3></center>

스토리 튜토리얼에 필요한 에셋들이 모두 제작되었습니다.이제 이 에셋들을 공간 안에 적절하게 배치시키는 것이 필요합니다. T4Framework은 프로젝트(Project)를 생성하고 이 안에 각 에셋들을 추가하는 것을 통해 자동으로 에셋들의 데이터베이스(DB)를 형성합니다. 각 카테고리에 맞는 에셋들을 추가하고 내가 원하는 위치에 직접 마우스로 드래그하여 배치하면 쉽게 스토리 콘텐츠를 완성할 수 있습니다. 프로젝트에 에셋이 등록되면서 자동으로 DB가 형성되기 때문에 추가적인 코딩 작업은 요구되지 않습니다.<br/>

아래에서는 각 에셋들을 프로젝트에 추가하는 방법에 대해 소개합니다.<br/><br/>

<h4> 1) Cave Entrance 설정 </h4>

<img src="https://user-images.githubusercontent.com/101547387/178391916-bf0402fd-7719-4e3c-90aa-6687b46fbce5.png"><br/>

Content Editor에서는 Project을 생성하여 에셋들을 배치하고, 각종 연출들을 추가할 수 있습니다.또한 완성된 콘텐츠의 최종 패키징을 진행할 수 있는 공간이기도 합니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/jBsq2vRFCUQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ CaveEntrance 에셋 배치 영상 ]</h4></center>

Content Editor에서 스토리 튜토리얼 시작 시의 플레이어 위치와 퀘스트 발동을 위한 존의 위치를 설정하였습니다.<br/><br/>

<h4> 2) Junkyard 설정 </h4>

<img src="https://user-images.githubusercontent.com/101547387/178395243-c7f00b93-1170-4cc6-b9bf-59ea59cbbf60.png"><br/>

Junkyard에서는 omE, 상자 그리고 TV를 배치하였습니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/j1173DvSvWw" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ omE 배치 및 Waypoint 설정 영상 ]</h4></center>

에셋을 불러와 omE를 배치한 후 이동 동선(Waypoint)을 설정해주었습니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/VwP4_ODNwGQ" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ 상자와 TV 배치 영상 ]</h4></center>
상자와 TV 에셋도 적잘한 위치에 배치해주었습니다.
<br/>
<br/>
<hr/>
<center><h3>- 스토리 튜토리얼 내러티브 (Quest) -</h3></center>

스토리 튜토리얼의 내러티브는 스토리 튜토리얼의 전체 이야기 흐름을 의미합니다. 스토리 튜토리얼의 내러티브는 처음 Pia가 등장하는 CaveEntrance와 로봇이 등장하는 Junkyard로 구성되어 있습니다. T4Framework의 Quest Flow 기능을 사용하면 등장인물과 아이템이 언제 등장할지, 대사는 언제 나오고 카메라는 언제 움직일지 등을 다양하게 설정할 수 있습니다. 코딩과 스크립트 작업을 필요로 하는 엔진과 달리, T4Framework은 대화, 행동 등 원하는 기능을 수행할 노드를 선택하고 내용을 입력하면 바로 실행시킬 수 있습니다.<br/>

아래에서는 스토리 튜토리얼을 구성하는 Quest Flow에 대해 합니다.<br/><br/>

<h4> 1) Cave Entrance </h4>
<h5> Quest Opening (타임라인 00:00~00:07) </h5>

<img src="https://user-images.githubusercontent.com/101547387/178398327-8d9c2eba-bf56-43ee-8bbc-7efc5ba1ba99.png"><br/>

스토리 튜토리얼이 처음 시작될 때의 QuestFlow 입니다.다양한 노드들로 퀘스트가 구성되어 있는 것을 볼 수 있습니다. 노드들이 조합되어 처음 진입 시 동굴이 환해지는 연출부터 동굴 안을 카메라로 비추는 연출, 주인공 Pia가 '양 옆에 길이 보인다. 어디로 갈까?'라고 대사하며 좌우로 두리번거리는 애니메이션을 취하는 부분이 실행됩니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/m9FLC9iEU2o" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Opening QuestFlow 제작 영상 ]</h4></center>

T4QuestFlow 기능을 사용하여 내러티브를 제작하였습니다. 드래그 앤 드로우로 내러티브 진행 순서와 어떤 연출/기능이 들어갈지 쉽게 설정할 수 있습니다.<br/><br/>

<h5> Left Exit & Right Exit (타임라인 00:11~00:27) </h5>

<img src="https://user-images.githubusercontent.com/101547387/178398372-d6359426-13b6-4586-bdda-f33a9f31ac39.png"><br/>

동굴의 왼쪽 길 또는 오른쪽 길에 도착하면 길을 따라 들어가볼지, 아니면 조금 더 둘러볼지를 고르는 선택지가 등장합니다. 길을 따라 들어간다는 선택지를 고르면 퀘스트는 종료되고 Junkyard로 이동합니다. 반면 조금 더 둘러본다는 선택지를 고르면 퀘스트는 중단됩니다.<br/>

<img src="https://user-images.githubusercontent.com/101547387/178398633-7699a4c0-1c1b-4c86-98e8-4f26d79f17d0.png">
<img src="https://user-images.githubusercontent.com/101547387/178399043-cf0208a4-f4db-4a9a-9ab4-a3fa52753231.png"><br/>

Branch 기능을 사용하면 두 개 또는 세 개의 선택지에서 각기 다른 결과가 연출되도록 설정할 수 있습니다.각 선택지를 골랐을 때 어떤 대사가 나올지 또는 연출이 등장할지 Quest Flow로 쉽게 설정할 수 있습니다.<br/><br/>

<h4> 2) Junkyard </h4>
<h5> omE와의 조우 (타임라인 00:30~01:05) </h5>

<img src="https://user-images.githubusercontent.com/101547387/178399077-8822e528-3da5-430f-9c8a-6896592514e9.png"><br/>

동굴 양쪽의 길 중 하나를 선택하여 이동을 하면 Junkyard에 도착합니다. 이곳에서는 상자를 찾고 있는 로봇(omE)을 만나게 됩니다. 로봇에게 상자를 건네주면 로봇은 상자를 들고 TV 앞으로 이동합니다.<br/>
<center><img src="https://user-images.githubusercontent.com/101547387/178399115-df443440-2900-4f74-9791-f693dc4c10fc.png"></center>

해당 퀘스트에서는 아이템을 소유하고 있어야만 퀘스트가 진행되는 조건을 설정하였습니다. HasItems 노드로 아이템을 지니고 있는지 여부를 확인하여 상자 아이템을 지니고 있을 때 다음 노드(Interaction)로 진행될 수 있도록 설정하였습니다. Pia가 지닌 상자를 회수하고 대사가 실행됩니다.<br/>

<img src="https://user-images.githubusercontent.com/101547387/175945429-bf1b9f9e-5f38-47d6-8eeb-fb4f26c3a840.png"><br/>

Action 노드를 통해 상자를 받은 omE가 이동을 하도록 설정하였습니다. 이 때 omE의 이동을 강조하기 위해 플레이어는 이동하지 못하게 하고, omE를 촬영한 카메라 워크도 함께 동작하도록 설정하였습니다.<br/><br/>

<h5> 엔딩 (타임라인 01:11~01:17) </h5>

<img src="https://user-images.githubusercontent.com/101547387/178399233-40838381-9f67-438f-8622-b45d4664657d.png"><br/>

로봇이 이동한 후 플레이어가 따라 들어갑니다. 로봇 앞의 TV 근처로 다가가면 화면에서 영상이 나온 후 동일한 영상(엔딩 영상)이 화면 전체에 플레이된 후 종료됩니다.
<br/>
<br/>
<hr/>
<center><h3>- 스토리 튜토리얼 연출 -</h3></center>

스토리 튜토리얼에서 사용된 연출에 대해 소개합니다. 로봇을 발견한 후 상자에 빛이 들어오는 것은 액션팩(ActionPack) 기능을 사용한 연출입니다. 또한 로봇이 TV를 향해 걸어갈 때 이를 뒤따라 가는 카메라 연출은 카메라 워크(Camera Walk) 기능을 사용한 연출입니다. 마지막으로 UI 기능을 사용하여 화면 전체에 미디어가 재생되도록 하였습니다.<br/>

아래에서는 액션팩과 카메라 워크, 종료 연출 기능에 대해 설명합니다.<br/><br/>

<h4> 1) 액션팩(Action Pack) </h4>

<img src="https://user-images.githubusercontent.com/101547387/178400444-49324593-9dd4-4fd0-ba03-1a8cee2ed0be.png"><br/>

Junkyard에 배치되어 있던 상자입니다. 상자 주변에 빛이 나는 것은 액션팩이 추가된 연출입니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/WNQV11MkvEI" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Action Pack 제작 영상 ]</h4></center>

플레이어가 omE 옆에 배치되어 있던 상자를 쉽게 찾을 수 있도록 상자 주변에 빛이 나는 액션을 추가하였습니다. 액션팩 기능을 사용하면 이러한 연출을 제작할 수 있습니다.<br/><br/>

<h4> 2) 카메라 워크(Camera Walk) </h4>

<img src="https://user-images.githubusercontent.com/101547387/178402405-04ff8b5e-1148-4206-9374-f5d7398e3c2d.png"><br/>

omE를 따라 이동하는 카메라입니다. 가운데 마네킹은 omE의 위치를 표시하는 마네킹입니다.우측 하단의 화면에서 카메라에 비춰지는 모습이 출력되며, 하얀색 선을 따라 카메라가 이동하게 됩니다.

<div class="embed-container"><iframe src="https://youtube.com/embed/S_b-dCgCefE" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ 카메라 워크 설정 영상 ]</h4></center>

Content Editor에서 Camera를 추가하여 원하는 Camera Walk 연출을 설정할 수 있습니다.<br/><br/>

<h4> 3) 종료 연출 (UI) </h4>

<img src="https://user-images.githubusercontent.com/101547387/179720384-63c57dec-1950-4b8e-b7a5-961c2dd258c4.png">

스토리 튜토리얼의 플레이 마지막에는 TV속 화면과 같은 영상이 화면 전체에 플레이되며 종료됩니다.<br/>

<div class="embed-container"><iframe src="https://youtube.com/embed/aJqvwNF_nTI" frameborder="0" width="1280" height="720"></iframe></div>
<center><h4>[ Ending UI 설정 영상 ]</h4></center>

준비된 영상을 Content Editor에서 엔딩 장면을 UI로 추가한 후, QuestFlow에서 언제 연출이 실행될지 설정하면(Junkyard 퀘스트 참고) 쉽고 간단하게 엔딩 연출을 설정할 수 있습니다.
<br/>
<br/>
<hr/>
<center><h3>- 스토리 튜토리얼 소개를 마치며 -</h3></center>

그동안 3D 콘텐츠 제작을 위해서는 언리얼 엔진에 대한 이해와 코딩에 대한 지식을 요구했던 반면, T4Framework은 보다 쉽고 빠르게 3D 콘텐츠를 제작할 수 있도록 도와줍니다. 저희가 소개해드린 스토리 튜토리얼은 T4Framework의 일부 기능을 보여드렸을 뿐이지만, 여러분의 손에서는 더 다양하고 무궁무진한 콘텐츠가 탄생할 수 있습니다.<br/>

여러분이 멋진 3D 콘텐츠를 제작할 수 있도록 T4Framework이 함께하겠습니다.
감사합니다. <br/><br/>

<center><a href="https://github.com/VirtualFlowInc/VirtualFlowStudio_Public/"><b>> 무료 평가판 사용해 보기 <</b></a><br><br></center>
<center><a href="https://t4framework.com/storytutorial_en/"><b>English</b></a> &nbsp;/&nbsp; <a href="https://t4framework.com/"><b>HOME</b></a></center>
