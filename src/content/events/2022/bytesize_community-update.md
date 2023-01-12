---
title: 'Bytesize: community updates Sep 2022'
subtitle: Phil Ewels
type: talk
start_date: '2022-09-27'
start_time: '13:00 CEST'
end_date: '2022-09-27'
end_time: '13:30 CEST'
youtube_embed: https://www.youtube.com/watch?v=KXXeAcHnDBo
location_url:
  - https://www.youtube.com/watch?v=KXXeAcHnDBo
  - https://doi.org/10.6084/m9.figshare.21222446.v1
---

# nf-core/bytesize

Join us for our **weekly series** of short talks: **“nf-core/bytesize”**.

Just **15 minutes** + questions, we will be focussing on topics about using and developing nf-core pipelines.
These will be recorded and made available at <https://nf-co.re>
It is our hope that these talks / videos will build an archive of training material that can complement our documentation. Got an idea for a talk? Let us know on the [`#bytesize`](https://nfcore.slack.com/channels/bytesize) Slack channel!

## Bytesize: nf-core community updates

The nf-core core team recently met for their first ever retreat. A lot of topics were discussed, in this talk Phil Ewels ([@ewels](https://github.com/ewels)) will describe the key points and cover some of the future directions for the community.

- New organisational team structure
- Updates to guidelines, test-data and archiving policies
- Looking ahead:
  - Subworkflows
  - awesome-nextflow pipelines
  - nf-core website updates

<details markdown="1"><summary>Video transcription</summary>
**Note: The content has been edited for reader-friendliness**

[0:01](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1)

thank you everybody for joining, this is a bit of a kind of last minute bite size that we've thrown into an empty slot that we had in the schedule and we thought we'd take advantage of that by telling you a little bit about what's happened in the past week or so with the nf- core community and some kind of updates which affect us all. This has been a little bit of a last minute talk even by my standards so apologies for it not being a very flashy slide deck but hopefully we can kind of talk through the different points and please feel free to drop something into a chat if you have any questions and or maybe Fran can relay any questions to me as I go along and this can be a bit of a kind of discussion bite-sized talk rather than just me presenting at everybody. Especially if there's anyone listening from the core team please do stop me if I get anything wrong or miss anything important.

[0:57](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=57)
The reason we have some updates for September is something a bit out of the ordinary happened last week, which is for the very first time the core team of nf-core got together, in person, because of COVID and the lack of in-person events we've had recently many people in the core team had never met one another in real life although we spend a lot of time online chatting to each to each other. And also over the last couple of years, especially as the NF-core Community has grown, when we do have in-person events at hackathons and things we're always so busy running the event that we don't really have any time to actually do any kind of core team work ourselves. So I kind of kicked this off this year for the first time that we'd have a little Retreat just for the core team, we're going to spend a few days getting to know one another and also trying to get through some some work for the core team and make some decisions and we'll really get into in-depth discussions about kind of Community scale things which are very difficult to take over slack and zoom. I'm glad to say it went really really well, we had a fantastic time, everyone came to kind of hang out in over in Sweden and we got to got to explore our surroundings and we went on a nice walk in the forest and everything. This is where this photo comes from. We played games in the garden and stuff like that and did also do a little bit of work. We managed to drop into Scilifelab and use a couple of offices there to spend a couple of days really, getting some work done. So we had our own kind of mini hackathon.

[2:40](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=160)
I looked over all the notes that we took over the days and broke out these these points which I'm going to talk over today. The first one's going to take up most of the time and I'll just kind of mention the others in passing. The first thing is "teams". We started nf-core end of 2017 starts of 2018. From very close to the start of that we had a core team, which is again, not very good naming -the nf-core core team - but all of you will know who we are we're quite visible and we have been kind of running the nf-core community. It's worked really, really well but the nf-core Community is getting bigger and bigger and bigger and the core team has got a little bit bigger recently but there's only so far that we can stretch ourselves. I've been feeling for a little while now that it'd be nice to formalize the community structure a little bit more, create some more teams and formalize responsibilities a little bit within those teams. We spent a good chunk of a day talking through all of this and which teams we'd like and how they'll be organized and what they should do. By and large we try to structure around what is already happening within the community. This means that it's pretty easy, we don't have to change very much and it there should be no real surprises, because this is basically how the community is already functioning. But we're just kind of hoping to formalize things, make things a bit more transparent and a bit clearer. All of this will go up on the website pretty soon, we just haven't got got there quite yet.

[4:18](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=258)
This is an overview. you can see the core team is still kind of at the middle but we have a handful of new teams here which are on this on this plot. The one which is completely new is a new Steering group. This is the top level of the community if you like. The Steering group won't do very much on a day-to-day basis but will be there to look after things like Finance. In the early days of nf-core we didn't have any Finance so we didn't really need to worry about that but with funding from Chan Zuckerberg Initiative and other actual Personnel working on the project now full-time we do have higher level decisions to be made. The Steering group will take charge of all the finance and all those large initiatives and think about some big picture planning.

[5:06](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=306)
The core team is basically remaining unchanged - same people - but again we're going to just write down what we actually do on a a day-to-day: running of the community, making decisions and generally we make decisions by kind of committee. If anything's not clear we take a vote and what we've said now that we have a steering committee is that if ever the core team is split, and there's no clear majority on a topic then we'll push that to a steering committee. I don't expect that to happen anytime soon, it's never happened in in the, what? Four? Four or five years that we've been running, but now we have a policy in case it does. The core team at the end of the day has administrative access to everything and another important task is they make final decisions on new pipeline requests and basically you know who should be within nf-core and how the nf-core pipeline Community runs. So no big changes there. We wanted to clarify membership a little bit again this is basically how we've been doing until now but we wanted to try and make that as transparent to the community as possible. It's a kind of a meritocracy, we basically invite people who have visibly been heavily involved in the Community and if if someone's interested in being part of the core team, then they can join. We want to try and make it explicit that we will try and have as best representation as possible to mirror the representation of our community.

[6:44](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=404)
There's a new team here called infrastructure. This one is kicking off with Julia and Matthias, basically because these two are now employed to work with nf-core as of this year which is fantastic! Julie is employed with Chan Zuckerberg initiative money to work on an nf-core infrastructure code and Matthias started recently at the Scilifelab data center to work on the same thing. Because I've been historically involved in this a lot I'm the lead of this team. This team will work purely on the tools code base on the website and any framework work around nf-core. Again, we've been working on this stuff for a long time already so there's no big change here but now we have an official team.

[7:35](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=455)
Outreach team has existed for a while but has been not super well organized and so we want to turn over a new Leaf with outreach. We've set some new leads: Chris, Marcel and Fran, and we will go over the membership of the the Outreach team soon and check whether people want to be involved and who wants to do what. We're also setting explicit responsibilities here and are hoping to pull back a lot. At the moment the core team does a lot of the Outreach work so we're trying to separate those two teams a little bit more now.

[8:11](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=491)
The safety team has existed for a while but it has not been super obvious to find this information. It's listed in the code of conduct and it has been working on a completely voluntary basis. Now it's still the same but now we have an official team which will be listed on the website. Saba, Michael and Chris have been doing a fantastic job for a year or two and now we're making it explicit that they are responsible for the code of conduct and they are the go-to people if there's ever any problems at either events or on slack. A key difference with the safety team is that they skip the core team and they will go straight to the steering committee with any recommendations if action is needed.

[8:59](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=539)
Another new team "maintainers". This is still in flux at the moment. We're thinking because basically until now everyone on the nf-core Community has been maintainers, everyone has full access to everything and everyone is expected to help out. This is not really the case. There are many people that are just not developing pipelines, they are just using them. Different people are involved to degrees have different levels of experience within nf-core. We're trying to add an extra tier in here where there's going to be an explicit maintainers Group which will be people that are not necessarily in the core team but who are heavily involved in maintenance work. This might be quite a big team and we want to try and do this so that we can scale uh with reviewing and pull-requests.
At the moment it's quite difficult to get a first release out for a new pipeline because we say that the core team has to review that first release, but there's not that many of us and there's lots of new Pipelines, so we're going to share this out a bit more if we can and basically share out some of this Maintenance task. This would be a really key for the nf-core community and more information will go out soon. We're going to come up with a list pretty soon of people we'd like to invite in the first round and we'll start rotating that list every six months and see how we go.

[10:20](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=620)
We'll see also how exactly we do this in the future but at the moment everybody has write access to every repository within nf-core. We may change that and we may make it so that most people have read access to most repos and then the main maintainers team adds people to the pipelines where access is required. This is just to streamline everything a little bit more and make sure the accidents don't happen.

[10:49](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=649)
For eagle eyed, you may have spotted the word ambassadors noted a couple of times. The ambassador's team will be a bigger extension of the outreach team and we have some pretty cool stuff planned. That's a bit too much to write here and it's not very well settled yet so just stay tuned. If that sounds interesting feel free to Ping us any questions but otherwise stay on the lookout and we'll be pushing some some more information out about ambassadors soon

right that's all the team stuff any questions before I move on.

[11:26](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=686)
um hopefully everyone's happy with kind of the decisions we've come to like I say hopefully there shouldn't be any big surprises here because this is pretty much how we're already operating. Enrique says the teams will get slack handles to be easy to contact so we'll set up some infrastructure around these teams

[12:03](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=723)
Some other thingswe talked through: The guidelines. A little bit about nf-core guidelines. They have been mostly untouched since the very start of nfcore um 2018. We've added a few bits over time and they were getting a bit unwieldy. The structure of the page, like some stuff with bullet points, some stuff with sections and some stuff was outdated and not really valid. Some bits we thought were missing so we've updated the guidelines page a little bit. Underneath docs and then contributing and then guidelines and so now the overview page lists all of them in one big list. Each requirement has a dedicated page with a bit more information just so that you can give space to dig into a bit more details about what we're talking about with the requirements, more than just a bullet point. It also gives you an overview at the same time, so hopefully this is helpful, we point to this page a lot. We're going to continue linking to specific things when it comes up in discussion and if you're developing within nfcore you should try and be aware of all the guidelines, especially if you're developing a new pipeline.

[13:17](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=797)
(Question) How do the guidelines influence existing pipelines?
Basically nothing's really changed and so there shouldn't be any changes. If you've got an existing nf-core pipeline, there shouldn't really be anything you need to worry about. We've made a couple of things a bit more explicit that we have previously been saying on slack anyway. Mostly we have just fleshed out more detail about the reasoning, like why does your pipeline name have to be lowercase without punctuation and why does it work like this way or that way. So it's mostly organizations of a page and more detail.

[14:01](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=841)
once you've had time to read through these and you know we're happy to take any questions and update and modifiers as appropriate.

[14:16](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=856)
Someone requested this I think this morning or yesterday: was there anything written about guidelines for reviewing?
This ties in with the new maintainers team as well that as we're asking more people to do reviewing. We need to better standardize how reviews should be done. We have some documentation already for the modules, I believe, about how pull requests should be reviewed and we're going to try and write up some more guidelines and some more help for this. We'll probably do a bytesize talk about it as well at some point, so this the aim of this is to standardize our reviewing process and also make it easier for new people to get into reviewing, which is a big big part of nf-core. It can be very rewarding in itself and is really critical to the functioning of the community.

[15:08](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=908)
Test data we talked about quite a lot. A couple of things are going to change. One of the things we're bringing in is a new requirement, that we want some more information about what test data is and we want that in a structured way. We're going to have a new requirement pretty soon for each test data directory to have a .yaml file and that .yaml file will have to have certain keys. This is to make sure that we know what the data is, where it came from, how it was prepared and everything. Because at the moment we're meant to have readme files but it's a bit hit and miss. Having the .yaml file will also allow us to add some continuous integration tests to be sure that those files are there and populated properly before a new test data is added. This will make reviewing a bit easier.
James has also written some new guidelines specifically for test data. You can find it under "docs", contributing, test data guidelines. This is an entirely new page spelling out what we had already been saying on slack, but in an informal way. Now everything's listed here for when you're generating new test data. This is how you should do it.

[16:27](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=987)
One of the things that came up several times is about maintenance and how do we do this, and when should we do it. We're very keen to try and make all of our plans scalable, sustainable not just "we should do that" and then forget about it. That's very easy to do. Therefore, one of the things we're going to try, and start doing, is do a bit of spring cleaning every year. James and Chris from record team are going to take the lead on organizing this and we'll send out reminders. The hope is that everyone in the community can just have a little think about this once a year and do do some tidying up. Things like looking at pipelines, to see if their pipelines are being actively developed. We have a handful of quite old pipelines, which were maybe started at hackathon years ago, and then abandoned. Other pipelines, which might no longer be maintained and maybe getting out of date. Things like looking for those and archiving them, where appropriate. We're going to write up some policies about how that process of archiving old pipeline should happen. And also just going through all the different pipelines and checking for old branches, which have been merged and can be deleted. Old pull requests which have been superseded, that are never going to be merged because it's already been done in a different way, curating the issue list, checking for things which have already been implemented, or duplicates... Just cleaning up all this stuff on GitHub. This is a constant thing that we should be doing over time, but it's just a good time to go, once a year, and say have a little focus on it and try and have a Community Drive on it. We tend to have hackathons in March, so we're thinking it's nice to do it a little bit before then, so that as we go into a hackathon we've got nicely curated lists of issues for people to work on and everything's fresh and ready to go.

[18:20](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1100)
There's a lot of published papers about nf-core pipelines. If you go to "Publications", you can see we've got a list of Publications here that we collect for all the different pipelines. If you didn't know about this, if you have a publication about a pipeline, whether it's dedicated specifically for that pipeline, or it just kind of describes the pipeline, please do add it to this page because it's really helpful to have it here. It's a bit of a difficult thing, because with nf-core we're a huge Community project. Especially when it comes to things like DSL2 modules, I could go and create a new pipeline today, import all these modules that other people have written, stitched them together and very quickly have a pipeline up and running. That would be great, but it'd be nice to be able to cite the people who've actually put in the work into those modules, the ones who actually wrote the code within the pipeline.
We are going to try and hit this head-on and try and write up some recommendations for how manuscripts and papers should properly acknowledge the community. We've already picked this up, it's obviously a Hot Topic and it'll be about where you should look for contributors. How you could potentially cite them. We might even come up with a little helper tool to automatically get a list of GitHub usernames and things like this. This will only ever be a helper tool for you if you're writing a paper, it's never going to be a hard requirement. We realize that Publications are highly political and very important for the people working on pipelines, at the end of the day, it will always be your decision about who you acknowledge and who you cite within your paper. This is just a bit of a helping hand, hopefully.

[20:10](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1210)
I want to give a shout out for a couple of slack channels. There is one that we created last week. We're talking about how to try and make the community as inclusive to new members as possible as one of the things that came up. It's easy to get an imposter syndrome, when you come and join a new slack, you join slack and there's always people chatting about things you might not understand if you're new to nexflow or new to the community. Then you feel like the question you've got is stupid and maybe you should be able to figure it out on your own. Of course that's not true! There is no stupid questions. If you're having a question, then chances are very high that other people have that question as well and that's what slack is for. We want to be as welcoming as possible and to lower that threshold we created a slack Channel specifically for this. The "no stupid questions" channel was based on another slack organization. I forget what the other slack organization was, but the idea is that this is a really friendly place to come and ask questions. You can find that on slack now. I think anyone who newly signs up to slack will join it but I haven't yet added the whole community. Please go and dig that out and have a look!

[21:30](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1290)
Another new channel, which I think is fairly freshly minted, which deserves everyone's full attention, is "nf-core memes", so go and have a look for there in your coffee break if you fancy it. Remember that there's the channel browser on slack. You have a look through there. There's a lot of channels on the nf-core slack, partly because we have one for every Pipeline. There might be some interesting ones hidden in there, so do have a poke around and see if there's anything in there, which might have been added or you might not have seen.

[22:00](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1320)
Final points. I will just to talk about the nf core website. Matthias especially has been working on this lately and will continue to do quite a lot of work on this. We've been doing a lot of planning work. First up, as you may have seen duplicate tweets appearing about releases or wrong times. I think we're pretty sure that's fixed now, so hooray! Next on the list is, if ever try and go to the stats page, you'll notice it takes a very long time to load, and if you're lucky it will load. If you're unlucky, it will crash and if you're really unlucky it might crash the website for everyone who tries to look at the website for a little while. This is not scaling well and as a top priority now we are trying to fix that, so that the website's a bit more nimble before all of the events we're having in a week or two. So hopefully we're going to get get that sorted very soon.

A few visual fixes and stuff coming up.
What we used to do for the pipelines is, in the documentation for the pipeline we used to have any number of markdown files, structured however you wanted. We decided a little while ago to try and standardize that to two files. Two files: "usage" and "output". That's good for standardization. It means it's easier to do template syncs, it's easier to build the website in a consistent manner. When you're used to looking at one pipeline or another, they will look the same. But we have found that there's a bit of pushback against that, because it limits you if you have a lot of documentation to write. Tor example if you want to write tutorials, or if you want to write pipeline specific stuff in more detail. Then it's useful to have more sub pages, so we're reverting that decision and we're going to soon open up the website, so that you can have any number of pages in the docs. You'll still have to have a usage and an output file as a minimum, but you'll be able to add others.

[24:08](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1448)
The big picture plan with the website is, we're going to do a big refresh, hopefully. At some point we're going to rewrite the whole backend, so it's much faster and scalable and actually built in a modern way. We're also going to restructure the website in a big way. We've got some plans where we're going to try and make all the documentation much easier to navigate, come up with a search bar which actually works and finds documentation within any pipeline or any parts of the website, and a whole load of big improvements coming. Please stay tuned.

[24:42](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1482)
That's all I've got! Two things I forgot to make slides about. One of them is quite a big one. Some of you may have noticed in the DSL2 modules repository there's a folder called "sub workflows", which has been quietly lurking here for a little bit of time. We worked quite a lot on sub workflows last week and made a lot of progress. This is coming and hopefully pretty soon. I was hoping I would talk about it a bit today, but I think there's some decisions which are still in flux, so maybe at the summit we might have a bit more to say about it. Certainly coming soon we will have subworkflows up and running, we hope. That includes both structure and everything within the nf-core modules repository. Also we got a proof of concept running for nf-core tools to work with sub workflows. That's really exciting! I know a lot of people have been looking forward to that, and working on that for a long time and I think we're getting close.

[25:47](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1547)
One other thing. I've already spammed everyone about this a great deal, so hopefully you've not been able to miss it. The nextflow summit is coming up and we also have a bunch of other events around that coming up. We have free online training, which is next week, which has got a ridiculous number of people signed up to it. It's completely taken us by surprise. I think we've got over 700 people now signed up to join the training, which is just fantastic! But there's always space for more, so if you're interested in getting some training, please do hop onto that page, get the details and register. It's the first time we've run it like this, where we're running in three different time zones at the same time. Running for three days for 2 1/2 hours. You can choose which time of day you want to run it in and that's really exciting. Then of course we've got the hackathon coming up in Barcelona and also online. We have also the main nextflow summit coming up as well. We've been updating the program a lot recently with different Speakers and things. We've got a keynote talk by Rob Patro, who's just put up his talk title last night. Lots of really exciting stuff happening there and I hope to see many of you there.

[27:04](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1624)
With that please ask me any questions or point out anything I've forgotten or got wrong happy to put more detail on stuff.

(Question) I was curious regarding test data. If you have discussed in in the core group and made a decision against the pull or whatever. What about having test data being built by pipelines themselves, because it can be quite tricky to for example, if you want to just add on to existing test data and process it further and create another output. It can be quite tricky to reproduce all the steps that have led to that old test data.

Absolutely! James mentioned this in the new documentation that he wrote. It is basically suggesting to do exactly what you're suggesting. If the test data for your module can be quickly generated, don't add that to the test data repo. Instead, in your test workflow, that you've got in the modules repo, add those other upstream modules to generate at each time. Bear in mind that that means every single time that module was tested it will be running those previous steps. Think about the polar bears a little bit. Think about the resources needed for the CI tests. If it's heavy lifting to generate those files then you should do it once and upload the file so I just download it and use. But if they're fairly quick to generate then absolutely don't feel like you need to add that to a test data repo instead, put it into the CI workflow.

(Question continues) I actually meant um what about starting putting pipelines into the test data repo then generate the test data
Pipelines are already in a test data sets pipeline repo. We've got a branch where we pipeline. That's how the CI tests run for pipelines. But I feel like that's not what you're asking. You mean generating test data sets.

(Question continues) exactly, having some kind of more reproducible definition of how to generate test data. Right now it's basically: put put the commands in in a readme in whatever it has data repo or branch. How about making that itself more reproducible by having (inaudible) pipelines.
I'm with you now. Yes, this is what this is about. At the moment we are not super happy with the the readme files, which is just massive readme files describing what all the files are and where it came from and how it was generated. We want to move away from this kind of readme file approach, where people can add as much or as little information as they want, to a structured documentation format. We're mostly thinking about origin, We haven't defined exactly what fields there are yet, so we could also define a command that was used to generate that test data if it originates from some other kind of file. We've got a "test data" slack channel so if you if you have something specific in mind hop in there and spell out exactly what you mean and we can discuss it in more detail and put something together.

[30:42](https://www.youtube.com/watch?v=KXXeAcHnDBo&t=1842)
good question. Something else?
core team you're happy that I haven't forgotten anything?
Maybe we should have it included more more photos.
Great. Okay, in that case let's wrap it up and thank you everybody for for joining and listening. It's been a real pleasure and a really fun week. I feel like we made tons of progress last week, so I'm really pleased. If you have any ideas or feedback on decisions we've made then please let us know and otherwise we'll continue writing everything up that we took notes on, adding it to the website and making it easily accessible for you.

</details>