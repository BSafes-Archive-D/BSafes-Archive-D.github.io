---
layout: default
title: Introduction
parent: § DDoS - From Activist Event to Perpetual Crisis 
grand_parent: D
nav_order: 10 
---
<style>
.dont-break-out {
  /* These are technically the same, but use both */
  overflow-wrap: break-word;
  word-wrap: break-word;

     -ms-word-break: break-all;
  /* This is the dangerous one in WebKit, as it breaks things wherever */
  word-break: break-all;
  /* Instead use this non-standard one: */
  word-break: break-word;
}

.youtube-container {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%;
}
.youtube-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

</style>

<div class="dont-break-out" markdown="1">

1. TOC
{:toc}

## Introduction
From March to October 2016 recurring attempts were made at blocking access to the official website of the organisation Black Lives Matter. <sup>1</sup> An Anonymous-affiliated team calling itself ‘Ghost Squad’ took responsibility for some of them, causing confusion on the part of commentators. <sup>2</sup> For many, it was unclear how to reconcile the thrust of these attacks with the political orientation of earlier actions of Anonymous such as campaigns against Scientology and in support of Julian Assange. Ghost Squad, specifically, had earlier targeted the website of the Ku Klux Klan. Yet in a video posted on May 2 on a YouTube channel called @anonymous_exposes_racism, the group explained that they had “seen people in your movement on the streets and social media chanting and posting slogans such as ‘Kill Whitey,’ ’Death to the slave masters’ and other objectionable statements,” and had, therefore, decided to take action: “We will not tolerate racist behaviour and hate speech from your movement or any other organization any more than we do from the KKK.”<sup>3</sup> Earlier, an account called, “s1iege” had tweeted screenshots of an ongoing Distributed Denial of Service (DDoS) attack along with the hashtag #OPAllLivesMatter. <sup>4</sup>

These events in 2016 raise many complex questions relating to the nature of online activism and to the specific circumstances of the fight for racial justice in the US. <sup>5</sup> While the full scope of these questions cannot be covered here, the attacks against Black Lives Matter provide an exemplary point of entry for thinking about changes in DDoS attacks as a political tactic. Blocking access to websites of political opponents

***
<sup>1</sup> Corin Faife, “The DDoS Vigilantes Trying to Silence Black Lives Matter”, Ars Technica, December 14, 2016, https://arstechnica.com/information-technology/2016/12/hack_attacks_on_black_lives_matter/. 
{: .fs-2}
<sup>2</sup> Catalin Cimpanu, “Anonymous Ghost Squad Hackers Take Down Black Lives Matter Website”, Softpedia, May 1, 2016, https://news.softpedia.com/news/anonymous-ghost-squad-hackers-takedown-black-lives-matter-website-503579.shtml. 
{: .fs-2}
<sup>3</sup> anonymous exposes racism, “Anonymous Calls out #BlackLivesMatter for Anti-White Racism,” YouTube Video, 3:01. May 3, 2016, https://www.youtube.com/watch?v=dDXsInz9jz8. 
{: .fs-2}
<sup>4</sup> Anonymous (@_s1ege), “#OpAllLivesMatter #GhostSquadHackers blacklivesmatter.com #Defaced and #Ddos’d ~s1ege” Twitter, April 30, 2016, https://twitter.com/_s1ege/status/726206708473847809. 
{: .fs-2}
<sup>5</sup> For investigations of these aspects, see Amber M. Hamilton, ‘A Genealogy of Critical Race and Digital Studies: Past, Present, and Future’, *Sociology of Race and Ethnicity* 6, no. 3 (2020): 292-301; Sarah J. Jackson, Moya Bailey, and Brooke Foucault Welles, #*HashtagActivism: Networks of Race and Gender Justice* (Cambridge, MA: MIT Press, 2020); Marcia Mundt, Karen Ross, and Charla M Burnett, ‘Scaling Social Movements Through Social Media: The Case of Black Lives Matter’, Social Media + Society 4, no. 4 (2018), doi.org/10.1177/2056305118807911.
{: .fs-2}
***

by means of DDoS attacks has long been considered a key tactic of online activism. <sup>6</sup> It represents a specific kind of induced crisis of communication that causes disruption in the flow of communication, thereby providing an opportunity to focus attention on certain issues. <sup>7</sup> However, as the example of Ghost Squad demonstrates, it is also a polyvalent tactic in the sense that the political (or commercial, criminal or plain malevolent) purposes affiliated with it can diverge widely and are prone to sudden shifts of political orientation.

One development that is especially apparent when considering the events in 2016 is that DDoS attacks have become a more enduring phenomenon. From early campaigns, which in many ways resembled traditional forms of political activism, involving a multitude of engaged people causing temporary disruptions that lasted for some hours or days, DDoS has turned into sustained cascades of highly automated attacks that can last for several months.

The aim of this paper is to spell out the consequences of this shift from DDoS as short-lived events to enduring phenomenon. The core argument is that this shift of temporality has repercussions on the distributional layers of internet infrastructure that have escaped the attention of existing scholarship on DDoS as an activist tactic. This point will be developed through three steps. First, the paper provides a technical overview of developments in the DDoS landscape. Secondly, this overview is related to established positions and periodisations in DDoS research. Thirdly, the discussion extends towards infrastructure studies in order to focus on the relationship between breakdown and visibility. The paper concludes by calling for a stronger engagement with the temporal aspects of recurring communication crises in general and DDoS attacks in particular.

***

#### Table of Contents
{: .no_toc}

<ul><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-1/">
Introduction</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-2/">
DDoS – Technical Developments</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-3/">
Phases of Hacktivism</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-4/">
Phases of DDoS: Technological developments</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-5/">
Effectivity and Legitimacy of DDoS</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-6/">
Breakdown and visibility</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-7/">
DDoS as breakdown</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-8/">
DDoS becomes ordinary</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-9/">
The politics of infrastructuring</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-10/">
Conclusions</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-11/">
Bibliography</a></li></ul>
***

</div>
