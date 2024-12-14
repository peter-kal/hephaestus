# hephaestus

Goals: Make a code editor, that's more complex than basic editors(like the Gnome one), but simpler than VScode.
For state management, BLoC will be used. For db don't know yet.
concept:
![](screenshots/Screenshot%202024-12-05%20211908.png)

- [ ] seeing a tree of the files of the directory at hand
- [ ] git support
- [ ] have terminal support(maybe use YaruPanedView)

# The Concept of Hephaestus

Hephaestus, taking its name from the ancient Greek god, is an effort to make a fully function and feature-proof code(and text) editor built with flutter. In this sort of article I would like to point out and describe the concept of Hephaestus, and the goals of it's development.

## As of Flutter

I believe a) that the Flutter coding ecosystem has reached the level of maturity to support the creation of a code editor, notable achievements have been the development of the re_editor package(the one that Hephaestus will use for the code editing part), which solves the perfomance issues of flutter_code_editor while not missing on features. Several attemps to create something similar have existed over the past years, for instance flutter_editor(looking at the repo this project seems dead, I will talk more about the sustainability of the Hephaestus project in a while), and Flutlab(a flutter code editor that targets the web, which as far as I know its closed-sourced and has different quality goals than Hephaestus, in case you were wondering why the reinvention of the wheel), this showcases that the material conditions for this are there. And b) that building a code editor with Flutter is a good deal, for quite some reasons, 1) it provides cross-platform availability, 2) Dart is a relatively easy programming language and Flutter is also popular, so contributions to the project, while also accounting the fact of cross-platform availability, should be prominent and more accessible, 3) Flutter apps are natively compiled so the performance should be better than Electron-based apps(this is only estimated through previous comparisons in apps of completely different nature, no real proof as of now 13/12/2024), like VScode. Theoretically speaking, using Flutter for building Hephaestus seems reasonable, and I truly think we will see more efforts to make a code editor with it, despite if it's Hephaestus that will make the cut or not.

## As of design choices

All code editors share a lot of same characteristics, which is logical because they all orbit around the goal of making devs able to code. Hephaestus takes and will continue to take inspiration from other and more popular projects like Elementary Code(the code editor built by the Elementary OS team), and VScode. That said development efforts won't be directed at making a good replica, for example, while VScode does have tabs, Hephaestus will not, you will be able to open multiple projects(folders), isolated files, and their git record, but they will only be accessible from the tree-view in the right/left side of the app. The theme of the app will also be in Yaru, developed by the Ubuntu/Canonical team which has done an outstanding job on porting flutter on desktop in a visually pleasing way. This allows removing the default title bar of flutter which is of no use, with the YaruWindowTitleBar, as well as constructing a look and feel more appropriete for desktop.
I hoped I could share more but Hephaestus is in an extremely immature phase, so without much of practice and experience, I can't move on, on lenghtening the theory behind it's development.

## As of sustainability

a)Previously, I stated the fact that an effort to make a project similar to Hephaestus has been inactive for over 2 years. Hearing something like that makes you question: Can we be sure Hephaestus will pass the test of time or not? And we should pose this question. Hephaestus unlike VScode, is not backed by a multi-billion dollars capitalist corporation, neither is has millions of existing users, it doesn't even have a small team like the Elementary Code. The only thing I can be certain are my development efforts. So the answer of the question a brings the question b: how much sure can we/I be on my dev efforts? Again I am not a big or even small entity, rather just a single developer, who to build Hephaestus has to learn many things from scratch, also I cannot say I will have a lot of time to spend on the Project, I have exams in few months that if they go well, I will also have to study for my University courses, and most propably I am also going to work. So the answer to question b is a strategy which holds in mind the not so flexible schedule of mine. I believe this is a slow development progress, spending a lot of time and energy, which I cannot afford to spare, on a project which needs a lot of time to be used and furthermore established on the dev community, is a wrong approach, I think this is the reason many projects fail and die. Playing the long game is the right decision, 'cause this is a long game, no code editor became known, used, and established among devs, in a night. Once the skeleton of the app is ready and published to Github, the development will be in a form of small, incremental updates. I don't have delulu hopes, and I expect Hephaestus will propably take some years before it reaches the state I imagine it to reach.
b) How will Hephaestus be established?
i)By established I mean to be relatively known and used, while also considered a safe, and stable solution for the goals and the problems it tries to solve. What are the goals? I hear you ask. A code editor that's not backed by a capitalist corporation, that's privacy-focused, that's fast and responsive, cross-platform, open-source, and as simple as possible while not missing features.
ii) after making the goals clear, there comes the time to lay out the strategy for hephaestus being well established.

1. Not releasing a stable version up until it is stable, and feature-proof enough, I have seen many projects release before they have ticked these boxes, they get bad first impressions, and those first impressions are very hard to get over, even after the project has become pretty good. I don't want Hephaestus to have bad first impressions, and thus I would try to keep low profile as long as I think it's not ready.
2. Any controversial feature, meaning any feature that hardly passes the goals stated, will either never be added or it will be added, but in a careful and opt-in way. For example I would like to add some LLM support to the Hephaestus to help people with coding, but considering the privacy-nightmare behind it, it will be an opt-in, and you will be able to access it only behind a security-privacy warning.

## As of the political stance

Everything is politics, even if you realise it or not, making something open-source is a political stance of it's own. But if Hephaestus passes the test of time, and it becomes popular, I would like to make clear that:

1. I condemn the Palestinian genocide, conducted by the terrorist state of Israel, backed by the USA-EU and the whole euro-atlantic capilist bloc. As a small try to express that(and I say small because the most powerful way is getting in the streets, is mobilizing against monopoly capitalism, and getting organised in Communist Party) I will try and block the access of the app as much as I can on Israel(Occupied Palestine) .
2. I am a Marxist-Leninist/ Communist, I condemn the capitalist system, I look forward to it's revolutionary overthrow, conducted by the working class and its social allies, farmers etc., and the construction of a world with no exploitation by man to man, socialism - communism. I also refuse to take part in the whitewashing of the american and in general Capitalist history, as well as the anti-soviet propaganda.
   So if in the future you see a post of mine that features this elements, don't be surprised.
