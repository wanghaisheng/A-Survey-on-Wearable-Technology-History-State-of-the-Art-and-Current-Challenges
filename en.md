```
Computer Networks 193 (2021) 108074
```
Available online 8 April 2021
1389-1286/© 2021 The Authors. Published by Elsevier B.V. This is an open access article under the CC BY license (http://creativecommons.org/licenses/by/4.0/).

```
Contents lists available at ScienceDirect
```
# Computer Networks

```
journal homepage: http://www.elsevier.com/locate/comnet
```
## Survey paper

## A Survey on Wearable Technology: History, State-of-the-Art and

## Current Challenges

## Aleksandr Ometova,∗, Viktoriia Shubinaa,e, Lucie Klusa,d, Justyna Skibińskac,a, Salwa Saafic,a,

## Pavel Pascaciod,a, Laura Flueratorue,a, Darwin Quezada Gaibord,a, Nadezhda Chukhnob,d,

## Olga Chukhnob,a, Asad Alia,c, Asma Channae,b, Ekaterina Svertokae,c, Waleed Bin Qaima,b,

## Raúl Casanova-Marquésc,d, Sylvia Holcerd,c, Joaquín Torres-Sospedrad, Sven Casteleynd,

## Giuseppe Ruggerib, Giuseppe Aranitib, Radim Burgetc, Jiri Hosekc, Elena Simona Lohana

a _Tampere University, Finland_
b _University Mediterranea of Reggio Calabria, Italy_
c _Brno University of Technology, Czech Republic_
d _Universitat Jaume I, Castellon, Spain_
e _University Politehnica of Bucharest, Bucharest, Romania_

## A R T I C L E I N F O

_Keywords:_
Wearables
Communications
Standardization
Privacy
Security
Data processing
Interoperability
User adoption
Localization
Classification
Future perspective

## A B S T R A C T

```
Technology is continually undergoing a constituent development caused by the appearance of billions new
interconnected ‘‘things’’ and their entrenchment in our daily lives. One of the underlying versatile technologies,
namely wearables, is able to capture rich contextual information produced by such devices and use it to
deliver a legitimately personalized experience. The main aim of this paper is to shed light on the history
of wearable devices and provide a state-of-the-art review on the wearable market. Moreover, the paper
provides an extensive and diverse classification of wearables, based on various factors, a discussion on wireless
communication technologies, architectures, data processing aspects, and market status, as well as a variety of
other actual information on wearable technology. Finally, the survey highlights the critical challenges and
existing/future solutions.
```
**1. Introduction**

Today, the rapid proliferation of the Information and Communica-
tions Technology (ICT) niche is being pushed by an increasing number
of new services and growing user demands. Generally, the number of
interconnected handheld devices has been growing tremendously from
year to year, empowered by both consumers and broad penetration of
the Internet of Things (IoT) [ 1]. Small, affordable, and very different
in shape, purpose, and application, the IoT devices had a tremendous
impact on the development of the telecommunications field, not only
bringing new long-range wireless technologies to the market, defining
new requirements in terms of reliability and availability but also push-
ing network operators and vendors to redesign the entire ecosystem,
switching from conventional human-generated traffics to more diverse
IoT one.
This tremendous impact on the ICT domain and proliferation of
the IoT allowed the developers to bring their attention to an entirely

```
∗Correspondence to: Tampere University, P.O. Box 1001, FI-33014, Finland.
E-mail address: aleksandr.ometov@tuni.fi (A. Ometov).
```
```
new market segment – a separate niche requiring standalone efforts
has emerged as devices carried by humans but no necessarily gener-
ating the human-type data. Internet of Wearable Things (IoWT) has
emerged as part of a broader IoT , bringing new challenges from various
technological perspectives to the research community [2].
The terms wearables , wearable devices , or also wearable technology
refer to small electronic and mobile devices, or computers with wireless
communications capability that are incorporated into gadgets, acces-
sories, or clothes, which can be worn on the human body, or even
invasive versions such as micro-chips or smart tattoos [3]. Compared to
today’s smartphones and tablets, the primary added value is that wear-
ables can provide various monitoring and scanning features, including
biofeedback or other sensory physiological functions such as biometry-
related ones [4]. Wearables can continuously measure such values —
```
https://doi.org/10.1016/j.comnet.2021.
Received 1 December 2020; Received in revised form 3 March 2021; Accepted 27 March 2021


```
Computer Networks 193 (2021) 108074
```
```
Fig. 1. Perspective on the development of personal wearable ecosystems.
```
restricted by their battery constraints; they are convenient, seamless,
portable, and can offer hands-free access to electronics.
The consumer-wearable devices of today are beyond their inception
but still very much in their infancy. Most people still use a combination
of an activity tracker and a smartphone, see Fig. 1 , limiting their
experience to the number of steps and heart rate. Indeed, the variety
of data collected and processed in a wearable ecosystem context can
hand over an unprecedented user experience for humanity [5]. In ad-
dition to conventional sports trackers, smartwatches, on-body cameras,
heart rate meters, and eye-wear, the upcoming generation of wearables
will also involve augmented-, virtual-, mixed-, and enhanced-reality
devices, various smart clothes, and industrial wearable equipment.
As foreseen by the ICT industry, almost 70% of early adopters have
shown their interest in correlating their lives with the next-generation
wearables [6]. Predominately, a significant portion of IoWT available
on the market today already provides a smartphone-like experience by
employing voice and gesture control together with well-designed input
and output interfaces.
Nonetheless, the miniaturization trend, portability, wireless commu-
nication, energy-efficient computing, and advanced display technolo-
gies have been combined to create state-of-the-art smart devices. The
patriarch of these devices, a smartphone, was released back in 1992 [7],
and intelligent media are now ready to lead the next great wave of
innovation. Comparing traditional smartphones with wearables, both
have their pros and cons. A traditional smartphone’s main advantage
is its higher accuracy in various performance metrics due to less power
consumption limitations as a general trade-off to size. On the other
hand, wearables are highly battery-constrained devices, yet have the
potential to change the world as we know it — just as mobile devices
did over the past 20 years. It is expected that they will improve the
technological and socio-cultural parts of our lives. Moreover, wearables
also have the strength to improve well-established sectors, such as
the smartphone industry and other hand-held devices. This trend is
confirmed by many recent studies and will be discussed in this survey.
From the monetary perspective, the wearable market is anticipated
to keep on growing exponentially in the coming years. The forecast is
at more than 20 % growth rate annually, and the market is expected
to reach over 40 billion EUR per year in the next 5 years with more
than 150 billion EUR by 2028 [8–10]. A recent number of wearable
shipments, estimated at 113.2 million in 2017 with total market size
of $70 billion in 2019 , is forecast to reach 222.3 million deliveries
yearly by 2021 [11,12]. Moreover, the outbreak of COVID-19 also
made a tremendous impact on the wearable devices evolution driven
by the implementation of various crowd-sensing and contact-tracing
platforms [13–16]. The proliferation of wearables is thus expected to

```
Fig. 2. Wearable market growth forecast [9].
```
```
steadily increase over the following decades, with a predominant transi-
tion from bracelets and sport trackers to smarter and more feature-rich
wearables. Wearable technology has a tremendous impact upon ICT in-
dustry, and smart wearables are expected to disrupt most personal and
business sectors, such as the industrial, healthcare, and sports domains.
Moreover, the global enterprise wearable market alone accounted
for over EUR 18 billion in 2017 , and it is predicted to grow at a
Compound Annual Growth Rate (CAGR) of 11.8% during the forecast
period,2019 − 2026[17]. The details on market changes as well as
future perspective [9] are given in Fig. 2. Here, wearable devices could
be used to improve employees’ physical activity, enable relaxation
more effectively, and increase workers’ safety and work efficiency [18].
Added value is also achieved in other sectors, such as smart city,
transportation, gamification, and infotainment. Wearable technology
relieves people from continuously having to hold their smartphones
in their hands from the usability perspective. This convenience feature
allows handling calls, emails, texts, and many other alerts without even
getting the bulky devices out [19,20]. Following Llamas’ work, ‘‘within
the enterprise, wearables can help accelerate companies’ digital trans-
formation by transmitting information back and forth while allowing
workers to complete their tasks faster’’ [21].
The mobile devices’ market growth brings new and usable devices,
numerous benefits, and new applications from the users’ perspective.
One of the primary stimuli brought by wearable technology is the
encouragement of proactive solutions to deal with healthcare, fitness,
aging, disabilities, education, transportation, enterprise, finance, en-
trance systems, gaming, music, and many others. Since wearables, as
known today, were historically planned as purely medical devices, let
us first consider an example from the healthcare field. Unfortunately,
people tend to deal with potential health issues reactively, e.g., when
they feel sick or in pain, they tend to appoint a visit to their doctor.
Carrying a wearable device may potentially forecast the disease by
continuous health tracking and even inform the doctor automatically
in order to take measures to prevent the incipient threat actively [22].
Even the simple activity trackers are already capable of monitoring
sleep patterns, heart rate, level of stress, or body temperature that could
be utilized for improving the health habits of any individual [23].
Significantly, the shift toward advanced devices, such as Augmented
Reality (AR)/Virtual reality (VR)/Mixed Reality (MR)/eXtended reality
(XR) devices, low-end wearables, and other monitoring devices, to-
gether with a transition to Beyond Fifth Generation (beyond-5G) mobile
networks would also bring several challenges for the device vendors,
network operators, and end-users. In particular, those challenges are
related to the paradigm shift from conventional Human-to-Human
interaction (H2H) to more Machine Type Communications (MTC) in-
teractions [24]. This segment brings completely different requirements,
```

```
Computer Networks 193 (2021) 108074
```
e.g., utterly different traffic patterns, higher reliability, lower latency,
highly mobile scenarios, stringent security and privacy needs, and
higher energy-efficiency demands than the H2H ones [25].
All of the conditions mentioned above lead to an indigenous in-
crease in power consumption and the need to recharge the wear-
able/handheld devices daily, reducing their attractiveness and limiting
the wearable applicability. Modern technologies, such as energy har-
vesting [26] and wireless charging [27], may assist in solving the
energy bottleneck, but the corresponding impact on the user’s health
has not yet been studied in detail [28]. Besides, energy harvesting
technologies are still far from mass adoption [29].
Overall, research in wearable technology is growing, which is
demonstrated, among others, by the number of publications in the
IoWT domain. Nevertheless, only one unified review is available to
the research community. In contrast, others have a particular focus on
some specific area (eHealth, sensors, adoption, etc.), while this paper
attempts to synthesize a standalone executive summary of various
technological aspects as well as related challenges. As of February
2021, the authors identified the following papers related to our survey,
i.e., at a comparable level of abstraction and topics’ coverage.
Several works have already reviewed materials, technologies, and
applications involving Wearable devices. One of the broadest and de-
tailed surveys was shown to the IEEE community in 2017 [30]. Ac-
cording to the authors, the paper has a _product survey_ style and is
mainly focused on the market-available wearable accessories, eTex-
tile and ePatches classification, and computing-, energy specifics, and
security aspects with a focus on present technologies. To note, close
to half of the paper deals only with the classification of wearable
devices available in 2017. A very recent review on wearable technology
and consumer interaction [31] introduced five main themes, includ-
ing decision-making, well-being; consumer behavior; utilities; and Big
Data analytics. Above all, they showed the lack of integration within
wearable technologies, which is driving to fragmentation, disconnected
terminologies, and studies that are not based on appropriate results.
The review performed by Xue et al. [32] introduced issues about
technologies, users, and activities with intelligent wearables. Moreover,
it identified the main risks (privacy, safety, performance, social and
psychological) involving wearables, which were also mentioned as hot
topics/themes for wearables in other related reviews [33]. The analysis
introduced in [34] focused on the current research highlights based
on nanomaterials and evaluated the electronics under the perspective
of actuators and sensors. The applications of Wearable Sensors were
analyzed for healthcare and human movement monitoring. In contrast,
the review introduced in [35] targeted the evaluation/assessment of
physical activity apps and wearables. They identified that 75 out of 111
analyzed works used in-device sensors to measure physical activity.
Numerous works specifically target the eHealth segment, e.g., the
work [36] dated 2015 provides an extensive overview of wearable
health-monitoring systems and related communication aspects sensors
and related implementation challenges. Another relevant work [37]
also covers the communication and architectural aspect of the eHealth
domain, extending [36]. Both are, however, strictly limited to this
particular segment. A cross-section of technologies for Sports and e-
Health was also assessed in [38]. The primary purpose was to evaluate
their reliability and suitability. They detected that most of the analyzed
technologies were not formally validated by an independent actor, and
only 5% provided a formal validation. The highlights provided in [39]
included the rising of wearables and the future for monitoring human
activity as well as biological signals.
Different from the other works, this paper provides a synergy of
various aspects of wearable devices from perspectives of communi-
cations, computing, localization, modern and future communication
capabilities and identifies challenges for each of the directions. As such,
it provides a standalone dataset of devices up until 2020, discussing the
aforementioned aspects without losing itself in (unnecessary) technical
details or device classification, as in [30].

```
In line with the discussions so far, the main goals of this paper are:
```
```
G1. To provide a detailed historical overview of wearable technol-
ogy evolution;
G2. To highlight the state-of-the-art in the field of wearable technol-
ogy, including mass-consumer perspective, main architectures,
market-available devices, and related technical classifications;
G3. To identify open challenges and provide a vision of future devel-
opments related to wearable markets and wearable computing.
```
```
The rest of the paper is structured as follows. Section 2 provides
a detailed insight into the history and development of wearables from
the early 13 th century till nowadays. Section 3 addresses the state-of-
the-art of wearable-technology evolution and outlines the main classifi-
cation, architectures, communication possibilities, and data processing
aspects of modern wearable devices followed by the main trends in
active wearable-technology development from both industrial and aca-
demic perspectives. Section 4 contributes by providing the list of main
open challenges and future perspectives. Section 5 concludes the paper
with a discussion summarizing the main findings of this work. The
appendix provides the results of the comprehensive market analysis
reflecting various types and models of wearable devices being currently
available on the market and under research.
```
**2. Historical perspective on wearables**

```
The wearables we know today are mostly treated as smart-by-
definition devices. People tend to forget that ‘‘smartness’’ has not
always been defined by processing the data on a chip, but rather by
delivering a better experience for actual users. The next subsections
give an overview of wearables’ evolution from the 13 th century to 2015.
The evolution is also graphically depicted in Fig. 3 for the ease of
perception.
```
```
2.1. Beforethe20thcentury
```
```
The journey of wearables started with the invention of spectacles
around the 13 th century by English friar Roger Bacon, who was based in
Paris and outlined the scientific principles behind the use of corrective
lenses in his Opus Majus (c.1266) [40]. Before R. Bacon, there had
been mentions of presbyopic monks using segments of glass spheres
that could be laid against reading material to magnify the letters (i.e., a
magnifying glass called ‘‘reading stone’’), but those are more question-
able in terms of actual wearability. Glasses by Bacon were the first
wearables designed to be seamlessly carried and improving the vision,
thus, becoming the pioneering smart glasses [41].
The first pocket mechanical watch, possible to be carried around,
dates back to the beginning of the 16 th century, and it is believed
to be the Pomander (Bisamapfeluhr in German) watch [42]. Peter
Henlein made it in 1505 as a portable but a not-very-precise clock.
This design started a hype in wearable watch development, followed
by more than ten different models in the next one hundred years [43].
Later on, pocket watches have also been developed significantly with
the evolution of miniaturization [44], which led to the idea of strapping
the device to the wrist in the 19 th century. Military needs primarily
drove the developments at that time [45].
From the smart ring’s perspective, the first known one is Abacus
Ring from the early 17 th century during the Qing Dynasty era [46].
Back then, a standard abacus was combined of 10 parallel wires located
between two boards on a frame with nine beads on each of them. It was
specially designed to be a compact smart accessory used to help traders.
It led the way towards modern wearable computers and, at the same
time, towards modern smart rings [47].
```

```
Computer Networks 193 (2021) 108074
```
```
Fig. 3. Milestones of the wearable devices evolution.
```
_2.2. Early_ 20 _thcentury_

The first step from the portable cameras’ perspective is the Pid-
geon camera, developed by the German inventor Julius Neubronner
in 1907 [48]. Unlike many other technological breakthroughs of those
times, the camera was designed to record Neubronner’s pigeon flights,
while this invention is sometimes mistakenly referred to as based
on military demands. It is probably because pigeon photography was
widely used during the first world war for aerial surveillance together
with airplanes [49].
Indeed, wearable development driven by the military during the
World War I-II period was enormous. In the first place, the first carried-
on wireless systems were redesigned for field communications [50].
Those were very bulky and, at first, used to be carried by cavalry horses.
A breakthrough in portable radio has been a ‘‘packset’’ system, which
later became known as a ‘‘walkie-talkie’’, developed in 1937 by Donald
Hings [51].
Wristwatches were necessary for the planning and coordination of
various operations, thus, enabling the mass adoption of wearables in
the prestigious military area [52] and, thus, allowing the marketing
teams to adopt wristwatches globally. Simultaneously, the first wired
hands-free devices integrated with flight helmets were being developed
for navy and pilots [53].
After World War II recovery, the next big step in the develop-
ment of wearable technology has been towards the VR by Morton

```
Heilig, who patented ‘‘Stereophonic Television Head-Mounted Display’’
in 1960 [54]. It was soon followed by another patent of the ‘‘Sensorama
Simulator’’ being an upgraded version of the initial device [55]. The
device was indeed the first VR simulator with a binocular display,
vibrating seat, stereophonic speakers, cold air blower, and an odors
generator [56].
```
```
2.3. Mid 20 thcentury
```
```
In 1961 , MIT researchers Edward O. Thorpe and Claude Shannon
concealed a timing device in a shoe that could accurately predict the
ball’s landing place on a roulette table. That became the first wearable
computer hidden in the shoe [57]. The real story behind the invention
was published later, in 1998 [58].
Just a few years later, Hugo Gernsback invented the TV glasses [59].
Those glasses weighed around 140 grams and were built around two
battery-powered cathode-ray tubes allowing for the stereoscopic expe-
rience [60], which was a breakthrough for 1963.
Next, in 1968 , Ivan Sutherland created the ‘‘Sword of Damocles’’
```
- known to be the first VR Head-Mounted Display (HMD) system,
enabling users to immerse themselves in a 3-dimensional environ-
ment [61]. The development has taken almost ten years while the
prototype was partially see-through and allowing head tracking.
    Inspired by Edward O. Thorpe, Alan Lewis invented the digital
camera-case computer to predict roulette wheels in 1972 [62]. Fol-
lowing Thorpe’s approach, he used a radio connection between the


```
Computer Networks 193 (2021) 108074
```
recipient of the information and the person. The recipient used a
computer to predict the roulette wheel and whispered the prediction
via a radio link to the hearing aid radio receiver.
A significant breakthrough in the development of smartwatches was
the appearance of the Pulsar Calculator Watch in 1975 [63]. The first-
ever market-produced calculator watch was retailed at a price as high
as $ 3 _,_ 950.
In 1977 , Hewlett Packard released its first algebraic calculator
watch [64]. The HP-01 was a genius of miniature and smart design
with 28 keys on the clock display. Four keys are raised for ease of use
(amount, alarm, memory, and time), and two were embedded, but one
could still use them using the fingers [65]. The rest of the keys were
important to press with a pen that instantly snaps the bracelet into the
clasp. The cheaper versions, mainly produced by CASIO, still ensure the
clock design of the calculator.
During the same year, the first camera-to-tactile vest was designed
by the company ‘‘Smith-Kettlewell’’ for the blind in 1977. It took a
decade of research. The device used a head-mounted camera to create
a tactile representation on 10 inches and 1024 points grid located on
the person’s vest [66].
The mid- 20 th century period could be concluded by one more
breakthrough in wearable devices – Portable Stereo Sony Walkman was
released in 1979 as the first commercially available portable personal
stereo cassette player with earphones [67]. Although it had two jack
outputs allowing for privacy, it was the first luxury wearable with a
leather case and stylish design.

_2.4. Late_ 20 _thcentury_

The wearable development in the 80 s passed relatively fast, mainly
driven by improving existing technology from previous years and a
new AR wave. In 1981 , Steve Mann had formalized the EyeTap project
and developed the first backpack-like computer designed to process the
data from a next-to-eye-mounted camera and showed it on the screen in
front of an eye [68]. That was the first step toward modern AR glasses
and the ancestor of Google Glasses [69].
The next massive acceleration of wearable computing development
was Seiko’s UC 200 WRIST PC introduction in 1981 [70]. It had 2 kB
of storage and offered the possibility to spell the time and calculation.
Despite that, a separate dock station and keyboard were available for
purchase.
Nelsonic Space Attacker Watch pioneered a new niche of portable
gaming in 1981 [71]. The watch was equipped with two buttons allow-
ing playing popular arcade games anywhere and anytime. After one
year, Nelsonic released portable Pac-Man and, later on, Super Mario
Brothers.
The second big father of Google Glass is the Private Eye head-
mounted display developed and sold by Reflection Technology in
1989 [72]. It had a monochrome monitor with a futuristic 720× 280
resolution for that time.
The beginning of the 90 s was lightened by creating The Active
Badge, the first portable indoor location tracker in 1990 [73,74]. It
was made by Olivetti Research and was suitable to transmit unique
Identifiable Infrared (IR) signals to communicate a person’s location,
which could be treated as the birth of the Smart Room concept.
Since the technological development pace was only increasing, Hip-
PC debuted by Doug Platt as a shoebox-sized computer just one year
later [75]. It was based on Ampro ‘‘Little Board’’ Extended Technol-
ogy module and, together with Private Eye and keyboard, formed an
Agenda palmtop. It already had a floppy drive and many additional
extenders.
Two years later, the development of widely known Knowledge-
based Augmented Reality for Maintenance Assistance (KARMA) has
started at Columbia University [76]. The system was also utilizing the
Private Eye for an overlay effect. This project’s main goal was to wire-
frame schematics and maintenance instructions on top of whatever was
being maintained.

```
The first steps for personal and portable electronic assistants were
made already in 1994. Mik Lamming and Mike Flynn developed
‘‘Forget-Me-Not’’, a continuous personal recording system [77]. It was
a technology that recorded the interaction with people and stored this
information in a database for future use.
In March 1996 , Palm launched the first-ever made mass-produced
personal digital assistant (PDA) – PalmPilot 1000 [78]. Being essentially
a one-chip computer, it has 128 kB of Random-access memory (RAM)
and up to 12 MB of storage. These devices received a 160×160 pixel
screen plus a stylus-based text input.
The year 1998 could be called the beginning of the wearable
payment epoch, currently present on Apple Watch and Android Wear.
The enabling device was the mBracelet [79]. It was a wrist-wearable
computer designed for financial transactions with Automated Teller
Machine (ATM). It had three slots that could accept interchange-
able iButton buttons. The connection between the mBracelet and the
host was through a three-color Light-emitting diode (LED) grid. The
mBracelet plug-in interface allowed users to exchange messages by
cross-shaking hands.
```
```
2.5. Early 21 stcentury
```
```
Levi’s Industrial Clothing Division (ICD) Jacket led the beginning
of the 21 st century, designed by Massimo Osti in collaboration with
Philips [80]. The jacket was made of technological material with an
internal network designed to interconnect electronic gadgets. The de-
velopment became revolutionary for its time and influenced the further
development of brands such as Acronym and Ma.Strum.
The year 2001 is the most known for introducing the first Plantronics
M1000 Wireless Headset, followed by the launch of the lightweight
M1500 version [81]. It was a combination of an M1000 Bluetooth
headset and an innovative Bluetooth mobile phone adapter that plugs
directly into the headset jack, giving all mobile users Bluetooth headset
freedom.
Fossil Wrist PDA met the market in 2003. Its development began in
1999 by Donald Brewer, who struggled to make the watch small enough
for the first year of development. He started the discussions with
Microsoft engineers looking for an over-the-wrist platform and con-
centrated on developing ‘‘Smart Personal Objects Technology’’ (SPOT
watches) [82]. After the size has been reduced enough, the screen was
attached. The first device had 2 MB of memory, which was expanded to
8MB for the commercial release. The price at debut was $249 US.
In 2004 , the first-ever GoPro camera met the world [83]. Nick
Woodman founded the company after surfing in Australia at 2002.
The first model was small, light, and waterproof while being AAA
battery-powered.
Later in 2006 , ‘‘Nike+iPod Sport Kit’’ was released [84]. It was a
device that measures and records distance traveled, pace, and more.
Nike+consists of a small accelerometer installed or already built into
shoes, which connects to a Nike+Sportband receiver connected to
Apple products.
Fitbit was founded in early 2007 by James Park and Eric Fried-
man [85,86]. In 2008 , Fitbit Classic was the first wireless activity
tracker that could synchronize data with the Internet and have the same
data available on a mobile phone. He was also innovative in the sleek
form factor.
In 2009 , Samsung S9110 Smart Watch was released. The company
continued Dick Tracy’s idea with a two-band wrist radio [87]. It was a
dual-band General Packet Radio Services (GPRS) phone with Exchange
email support. Samsung S9110 Smart Watch was the first smartwatches
that included a full-color touchscreen, Bluetooth connectivity, music
player, and voice recognition feature [88].
In early 2012 , Eric Migikovsky thought about a device that could dis-
play messages from selected smartphones (Android and Apple devices)
after creating the company Inpulse (Allerta) [89]. The initial version of
the watch was attractive by the bold and original design. Moreover, it
```

```
Computer Networks 193 (2021) 108074
```
was easy to read in daylight on the ‘‘smartwatch’’ [90]. The design was
highly accepted by the Kickstarter community [91]. After a few gen-
erations of watches and its acquisition by Fitbit, Pebble was removed
from the market, leaving the niche of e-paper display-based watches
abandoned.
In April 2012 , information about Project Glass appeared on the
Google Plus social network. The first post of the account was about the
project’s goals: to build a portable computer that will help ‘‘explore and
share the world’’. A video called Project Glass was attached to the post
with the project [92]. Soon after Google showed the concept, people
saw the glasses in real life. Google co-founders Sergey Brin and Larry
Page put on glasses in late spring 2012. At the Google I/O event on
June 27 , 2012 , Google showed technology in action to a public audience
under the price of $1500 [93]. This milestone is the beginning of VR
and AR mass adoption.
The year 2014 could be described as the period of personal activity
trackers boom. As a continuation and improvement of Fitbit’s story, the
most advanced device of that time, Basis, differed from other fitness
ranges by collecting data such as heart rate, calorie consumption by
activity, several sleep stages, and sweating and skin temperature with
Body IQ technology [94]. The market faced numerous projects, and the
number of people wearing those went sky-high in just a few years [95].
A standalone invention of 2014 was Tommy Hilfiger’s solar power
jacket to charge the phone [96]. Solar batteries were sewn into the
jacket, connected, in turn, to the battery, which was located in one of
the front patch pockets. Two devices could be connected to the battery,
for example, a mobile phone or a tablet. Moreover, solar panels could
be easily detached.
The next breakthrough for end-users was later in 2014 by intro-
ducing Android Wear (currently known as Wear Operating System
(OS)) [ 97]. This marked the time when the first industrial giant of-
ficially stepped into wearables. Wear OS was the first operating sys-
tem specifically designed for wearable devices, particularly for smart-
watches, and was the beginning of Google’s move towards taking a vital
position in the wearable market.
Pushed by the technological race, Apple released its first wearable,
Apple Watch, in 2015. While Google was mainly aiming at the market,
the Apple Watch story has a more tragic background [98]. Before 2011 ,
Steve Jobs had long and unsuccessfully fought pancreatic cancer, and
experienced the healthcare industry’s imperfection in the United States
firsthand. He saw how inconvenient it was for the nursing staff to com-
municate with patients, how difficult it was to monitor an outpatient’s
condition and retrospectively collect the necessary information about
the time spent outside the hospital. It was then that Steve Jobs decided
that medical care could be improved with technology, and Apple should
solve the problem of collecting and structuring data. Existing activity
trackers were not suitable for monitoring patient conditions daily.
That is why Apple came up with the Watch. The integration with
a powerful software and cloud platform was supposed to facilitate
doctors’ work. Sadly, Steve Jobs passed away four years before the
device was released.
The evolution of wearable technology during the period from 2015
till now will be covered in the next section as a state-of-the-art and
market overview.

**3. State-of-the-art and related work on wearable technologies**

This section overviews the current situation in the wearable technol-
ogy development domain. First, it provides the primary classification
types of wearable devices in Section 3.1 followed by the underlying
architectures in Section 3.2. Further, we list the data processing and
computing techniques in Section 3.3. The discussion on currently avail-
able and developing wearable communication technology is provided
in Section 3.4. The inseparability aspects from the wearable technology
perspective are highlighted in Section 3.6. Section 3.7 shows an actual
review of the leading wearable technology research directions from
both academia and industry. Finally, this section is concluded with a
list of the main directions driven by the mass market.

```
Fig. 4. Classification of wearable devices based on the on-body location.
```
```
3.1. Varietyofwearabledevices
```
```
Generally, the classification of wearable devices could be outlined
from various perspectives based on various factors. Interestingly, de-
vices worn and carried can have similar functionality but completely
different form-factors, technology levels, different on-body locations,
etc. Thus, the broadest classification is based on the application type,
even though the other classification groups may significantly overlap.
One of the broadest classifications corresponds, but is not limited, to
the following application/functionality types (discussed in more details
in Section 3.7 ), and sorted alphabetically in Table 1.
Another significant factor for classification is related to the de-
vice type (without relation to the application area). The types are
systematized in Table 2 and sorted alphabetically.
The variety of types could be broadened even further by decreasing
the level of generalization. This subsection lists the main concepts
present in the market and studied in the literature.
From the broad adoption perspective, the most intuitive consumer
classification factor is related to the placement of the wearable on
the human body. Here, the main groups (concerning device type) are,
see Fig. 4 :
```
- Head-mounted wearables: Those are mainly focused on percep-
    tion and control aspects. The group related to vision covers:
    AR/VR/XR/MR glasses, relaxation masks as well as HMD and
    personal entertainment systems. Audio-related devices include
    headsets, personal assistants, bass systems. A standalone group is
    related to neural interfaces.
- Body-worn devices: Those have much broader functionality and
    could also be divided into the following subgroups:


```
Computer Networks 193 (2021) 108074
```
**Table 1**
Classification based on the wearable application/functionality types (sorted alphabetically).
Type Brief description
Communication functionality (C) Provides the potential not to process the data locally but to exchange it with surrounding nodes and/or remote
cloud.
Control/input functionality (CI) A broad area of input devices ranging from smart buttons to sophisticated gesture recognition devices. This
group’s main task is to extend conventional Human-Computer Interaction (HCI) input focusing on the usability
of the devices keeping a small form-factor as a rule.
Education and professional sports (ES) Aim at improving the education and training by monitoring assistants.
Entertainment, gaming, and leisure functionality (E) The improvement of the perception experience include, e.g., audio systems, personal entertainment displays, etc.
Heads-up, Hands-free Information (H) Extend the conventional ways of the data delivery to the user utilizing personal assistants, AR, XR, Remote
Expert Devices, wearable cameras, etc.
Healthcare/medical functionality (HM) Separated from conventional sensing and monitoring ones due to the need to obtain medical device status that
requires significant effort in the device development and testing as well as providing a high level of the
obtained data trustability and the need for additional certification, however, covering similar devices, e.g.,
Electrocardiogram (ECG), Electroencephalogram (EEG) monitors, relaxation devices, neural interfaces,
exoskeletons, etc.
Location tracking functionality (LT) Requires to have either some Global Navigation Satellite System (GNSS) on board or, at least, a wireless
communication technology. On the one hand, the concept here corresponds to location awareness from the
node’s perspective and, on the other hand, to remote localization of the device if needed.
Notification functionality (N) Ranges from simple vibration notification to complex AR extensions. Similarly to sensing functionality, almost
any personal device connected to the cloud directly or via the gateway can carry this functionality.
Output functionality (O) Various visual, audio, or haptic-enabled devices to provide the user and/or people around with prompt
information from the personal ecosystem.
Safety and Security functionality (S) Personal safety devices, emergency assistants, etc.
Monitoring functionality (M) Extremely straightforward and cheap to implement this functionality. Generally, any device that has an
accelerometer on board can already provide some level of sensing. (Fitness and preventive healthcare —
Activity Trackers, ECG, EEG monitors, etc.)
Wearable devices for pets and animals (PF) Mainly covers smart collars, bark collars, smart clothes, etc.

**-** Near-body and Sport: A segment for the devices supplement-
    ing existing wearable ecosystem, such as e-patches, smart
    bands, supplementary activity tracking sensors, etc.
**-** On-body: EEG and ECG monitors, posture correcting de-
    vices, safety devices, various smart clothes, etc., form this
    subcategory.
**-** In-body: The most significant niche from a medical perspec-
    tive includes implantables, smart tattoos, etc.
- Lower-body devices: This group is still in the infancy but al-
ready includes some wearables such as smart shoes, belts, insoles,
etc. Most of them carry specific monitoring functionality for
professional sport or medical purposes.
- Wrist-worn and handheld wearables: Those are the most widely
adopted and market-filled niche covering smart rings,
wrist bands, smartwatches, gesture control devices beyond others.

The wearable-placement classification is one of the most natural
ones. Designers, researchers, and early integrators should carefully
consider that their device’s placement is selected appropriately to fulfill
the application requirements listed in the previous subsection.
In addition to the classifications mentioned earlier, wearables can
also be classified based on their energy-consumption profile. Usually,
devices with displays are comparatively more power-consuming than
ones without a graphical output interface [2]. However, it also depends
on the nature of the application and the extent of processing they per-
form. Therefore, wearables can be broadly classified into low, medium,
and high-power wearables.

- Low-power wearables are mostly devices involving low-power
    components with limited capabilities that need to operate for a
    longer time, mainly for data acquisition/sensing purposes. These
    may include different healthcare-related wearables requiring low
    data communication rates. For example, a smart ring for sensing
    human physiological parameters can be classified as a low-power
    wearable since it is a compact device with a small battery, radio,
    and a few sensors onboard [168].
       - Medium-power wearables include devices that may have a small
          display with slightly higher capabilities than low-end wearables.
          They can also have multiple sensors on board with direct or
          indirect internet connectivity options demanding medium data
          rates. These devices include smartwatches, fitness trackers, and
          other gadgets for activity/gesture recognition applications for
          individual, commercial, and industrial purposes [169].
       - High-power wearables include devices that are more power-
          hungry since they include heavy processing units demanding
          high data rates and large displays capable of performing dif-
          ferent compute-intensive tasks such as real-time image/video
          processing, Machine Learning (ML), etc. Examples include various
          headsets, glasses, head-mounted cameras for video crowdsensing,
          and others [170–172].

```
Wearables could also be classified based on the type of battery they
use. Currently, there exist three different types of Lithium batteries
available to be used in wearables thanks to the lightweight and high-
voltage characteristics of Lithium [173]. Lithium Coin, also known as
button cell batteries, are one of the earliest batteries developed for
wearables such as watches, remote controls, etc. They are lightweight,
low cost, and compact in design, mostly similar in size and shape to
a coin. However, these were non-rechargeable and disposable batteries
that needed to be replaced once depleted, which increases the e-waste
problem [174]. Lithium-ion batteries are the most commonly used
in wearables such as smartphones, smartwatches, fitness bands, etc.
They are rechargeable, lightweight batteries with high-power density.
However, the downside is that they are not very safe for wearables
since these devices are in close contact with the human body. There
have been instances where Lithium-ion batteries of smartphones have
exploded due to overcharging/heating. They require special circuitry to
ensure safe operating voltage and current. Moreover, their performance
degrades over time, even if not used [173]. Lithium Polymer, also
known as the Lithium-ion polymer, is rechargeable, lightweight, and
comparatively safer than Lithium-ion. However, it is costly with a
slightly lower power density than the Lithium-ion [175].
```

```
Computer Networks 193 (2021) 108074
```
**Table 2**
Classification based on the wearable device type (sorted alphabetically and application types abbreviations are from Table 1).
Device Refs. Apps. Power Prof. Brief description
Activity
trackers

```
[99,100] C, H, LT, N, S,
M, PP
```
```
L-M Simple and relatively cheap devices mainly focus on everyday activity monitoring, including the
number of steps, basic heart rate, and/or body temperature data collection. The main goal is to
increase the overall physical activity participation of an average user.
AR devices [101–104] C, CI, ES, E, H,
LT, N, OP
```
```
H Augmented reality applications can provide additional ‘‘seeing with more eyes’’ information that
cannot be displayed and is usually hidden from the observer in a see-through manner. The most
attractive areas of the AR development are related to tourism, exhibitions, and manufacturing.
Audio
systems
```
```
[105,106] C, E, H, N, OP M-H Conventional wired and wireless headphones, bass systems, as well as hearing aids. Moreover,
high-quality wearable audio could be integrated as part of XR or MR system to improve the
immersion.
E-Skin (or
nano
patches)
```
```
[107–109] C, CI, M, PP L An artificial skin with mechanical properties of human skin, providing various sensing functions with
the main application area of artificial tactile systems. It is commonly located either right on the
human skin or the arms of robotic systems to provide close-to-human perception abilities, e.g., to for
the operation of humanoids.
E-Textiles
(smart
fabrics)
```
```
[110,111] C, CI, ES, N, OP,
M, PP
```
```
L-M It is very similar to the e-Skin concept but broadens the opportunities to any close-to-the-body textiles
that incorporate electronic functionality. Here, the sensors, circuits, or input/output devices are
directly integrated with the fabric, allowing for seamless integration of the technology into everyday
garments.
EEG and ECG
belts
```
```
[112–114] C, ES, M, PP L-M Allow monitoring the user’s health state from both fitness, medical, and professional sports domains,
potentially without the need for specialized medical equipment.
FPV, HMD [115–117] C, ES, E, H, N,
OP
```
```
H Devices for full immersion of, e.g., the Remote control (RC) of various robotic systems teleoperation,
human interaction, e.g., police or firefighters, and/or conventional movie watching.
Haptic suits [118–122] C, CI, ES, E, H,
N, M
```
```
H Haptic feedback and capture both motion and biometrics features devices. Full or partial body haptic
feedback systems are built into the suit and can be engaged in actions, on-demand, or in response to
motion capture comparison to provide deeper immersion in various reality applications.
Ingestible
and
insertibles
```
```
[123,124] C, M, PP L-M Objects that go in, through, and underneath the human body or may be a size of a medicine capsule
and are packed with sensors, microprocessors, controllers, etc. Ingestibles are considered the next step
of wearable technology and used in healthcare for disease diagnostics and monitoring.
Location
tackers
```
```
[73,125] C, ES, LT, N, S,
M, PP
```
```
L-M Functions of remote position estimation of the user. Those are of specific interest for pet owners and
parents besides the historical crime-oriented market.
Neural
interfaces
```
```
[126–130] C, CI, H, N, OP,
M, PP
```
```
M Allow for a completely new experience in HCI for both complex medical states of the patients with
movement disability, treatment of tactile function, behavior monitoring, and gaming.
Personal
notification
devices
```
```
[45,87,97,98] C, H, LT, N, OP,
S
```
```
L-M Those could be considered as one of the earliest areas of mass wearable devices. When the first
activity trackers received an embedded vibration motor and Bluetooth communications, it became
possible to send a simple sign to the user about the incoming call or received message. Today, we
cannot imagine almost any wrist-worn device without this function.
Portable
Radio
```
```
[50–52] C, CI, H, LT, N,
OP, S
```
```
M-H Those devices were also taking place in the wearable devices evolution back in the first part of the
19th century. Starting with walkie-talkies, we have arrived at the era when surviving a day without
your smartphone could be problematic.
Relaxation
masks
```
```
[131,132] C, M L-M This group is an interesting set of devices that could be affiliated with luxury or medical purposes
but keep the same function of improving the sleeping experience. The devices could also be suitable
for people who travel a lot to improve the day-time adaptation period after, e.g., jet lag.
Safety
buttons
```
```
[133,134] C, CI, LT, N, S,
M
```
```
L This group corresponds to a specific set of notification devices but operating vise-versa, i.e., aiming to
notify either some special units, e.g., police or hospital or the user’s relatives, if something is
happening with the owner.
Smart Bands [135–138] C, ES, H, LT, N,
S, M, PP
```
```
L-M Carry the functionality of modern activity trackers but sometimes also provide gesture recognition,
stress/mood detection, or ECG monitoring functionality.
Smart clothes [96,139–141] C, CI, ES, E, H,
LT, N, OP, S, M
```
```
M-H A broad segment coupling together various common-looking clothes, ranging from pants to scarfs, but
with invisibly embedded features, such as heating, charging, displaying, etc.
Smart contact
lenses
```
```
[142,143] OP L Devices to boost vision and monitor physiological parameters that help track blood glucose level from
the body fluid, i.e., also tears intraocular pressure, with the help of the electronic device’s resistance
and capacitance.
Smart
footwear
```
```
[144–146] C, CI, ES, E, LT,
M
```
```
L-M Insoles, shoes, and socks are commonly used to monitor a person’s posture, gait, a number of steps,
beyond others, and are mainly utilized for training professional athletes from monitoring and
stimulation perspectives and monitoring of children.
Smart gloves [139,140,147–149] C, ES, E, H, M L-M Another hand-held type of wearables is commonly utilized for systems requiring either sophisticated
gesture recognition, rehabilitation, or providing better haptic feedback and other wearable devices.
Smart
necklaces
```
```
[150–154] C, LT, N, S, M L-M Luxury jewelry with activity tracking, health monitoring, posture correction, or safety functionality.
This group of devices did not find much attention due to the actual need for miniaturization and
keeping the appearance high.
Smart
patches
```
```
[108,155–157] C, M L Nodes consist of a peel-and-stick disposable part that is adhered to the skin and reusable sensor parts.
Smart patches are easy to attach, maintain, and remove, acting as an example of Wireless Body Area
Network (WBAN) system utilized in sports and healthcare monitoring.
Smart rings [46,47] C, CI, ES, E, H,
LT, N, OP, S, M
```
```
L Similar functionality as activity trackers but in a smaller form-factor and without displays. Some smart
rings also have a notification device functionality but are kept in a fashionable accessorize form.
( continued on next page )
```

```
Computer Networks 193 (2021) 108074
```
**Table 2** ( _continued_ ).
Device Refs. Apps. Power Prof. Brief description
Smart tattoo [158,159] C, ES, M L A set of biosensors implanted under the skin that measure glucose levels and change color depending
on the result. Smart tattoos promise to make life easier for people with diabetes and become an
alternative to permanent blood collection from the finger.
Smart
watches

```
[45,97,160] C, CI, ES, E, H,
LT, N, OP, S,
M
```
```
L-M The most widely adopted wearables after the activity tracker. Generally, it provides almost the same
functionality as a smartphone. However, most smartwatches’ energy efficiency is still challenging
without the gateway node due to the small form-factor.
VR/XR/ MR [161–166] C, ES, E, H,
LT, N, OP, M
```
```
H Visual immersion in the virtual environment with well-progressing VR applications being
entertainment, education, and healthcare. MR are a particular subset of VR that involve merging the
real world and the virtual world somewhere in a ‘‘continuity of virtuality’’ that augments completely
real environments to virtual ones, as defined in the basic work. Interestingly, the relatively new
concept XR is currently trying to unite all previously known reality-related paradigms.
Wearable
cameras
```
```
[116,167] C, LT, OP, M,
PP
```
```
M-H Devices are utilized by special units and athletes to record the environment for future analysis or via
real-time streaming.
```
Indeed, the modern wearable electronics market is extensive, and,
thus, the device classification approaches are also manifold. In this
subsection, we have listed the most significant ones and also briefly
highlighted less popular directions. The following sections provide
more details on the devices’ specifics and could also be considered an
extension of the traditional classifications.

_3.2. Architecturalaspects_

Typically, wearable devices use the owner’s smartphone as a gate-
way to connect to the Internet. Therefore, operational efficiency may
be limited if the gateway battery is empty or the connection options are
insufficient. Currently, some wearable devices have a long-range wire-
less radio. However, continuous use is still not recommended due to
high power consumption [2]. The evolution of wearable architectures
is shown in Fig. 5.
Historically, legacy eHealth systems were based on a few specialized
devices, such as biomedical sensors, worn by the patient, and on some
storage and computation facility, either local or remotely located in
the Internet [176] – the first architecture of wearable devices is a
separate device. In such systems, wearables are allowed to monitor
the users’ status by collecting information ranging from physiological
signals (e.g., heart rate, skin temperature, and physical activities) and
their interaction with everyday objects.
At the next step of the architecture evolution, wearables became
connected to more powerful external devices via wired links for data
processing tasks that cannot be executed on the wearables due to
their form factor limitation (Fig. 5 A). Such architectures, mainly in
healthcare-related applications, restrict user mobility, which is consid-
ered an obstacle to expanding wearable solutions. The key to smart
healthcare services is the ability to track patients’ health conditions
without the need for frequent visits to medical centers or hospitals
and provide real-time alerts in critical situations [177]. As a result,
traditional wired health monitoring systems have been replaced with
wireless wearable systems.
Due to the mass adoption of smartphones being a part of the
personal wearable cloud, manufacturers started to aim at other con-
sumer wearables as supplements in a personal ecosystem rather than
standalone devices. It resulted in a new architecture where personal
smartphones act as relays or gateways to transmit the data to the cloud
either directly or with pre-processing in the custom applications. Fur-
thermore, this architecture is supported by IoT technologies capable of
bridging in the proximity of the users to a multitude of general-purpose
smart devices. These IoT devices allow to gather further information
concerning the environment surrounding the user and adapt it to the
user’s needs.
According to the IoT architecture provided in [178], the gateways
are also called monitoring stations that are part of the perception layer
for people with disabilities. Logically, with the development of personal
wearable clouds, the logical star-like topology was supposed to join the
communications (see Fig. 5 B). However, due to the broad adoption **Fig. 5.** The development of wearable architectures.


```
Computer Networks 193 (2021) 108074
```
```
Fig. 6. Wearable data processing.
```
of Bluetooth technology as a leading connectivity enabler, wearable
devices started to communicate purely in a centralized way using the
gateway devices as masters.
Most fitness, sports, and healthcare wearable applications follow
the fourth evolution step in Fig. 5A, while sharing their data with
applications installed on the smartphones. This option implies several
situations where wearables cannot connect to the network, such as
the nonexistence of a smartphone nearby, non-installed applications
on the smartphones, or an outdated phone software [179]. Considering
such possible scenarios and the end-users ever-increasing expectations
and needs, device manufacturers consider equipping wearables with
short-range and long-range connectivity chipsets. As a result, these
standalone wearables can function independently from other devices.
Although this standalone wearable-based architecture provides a
way towards separating wearables from other personal devices and an
opportunity to communicate directly with the cloud, it brings some
challenges in terms of network design and dimensioning. For instance,
additional loads on the wireless networks are expected due to the lack
of pre-processing, usually performed by the gateway devices. Another
challenge is related to the deployed communication technologies op-
timized for low-power operation, thus, long battery life and reduced
device complexity.
Today, most wearable devices have at least two wireless interfaces
on board. The trend of unifying the operation is expected to push
vendors to add more wireless modules, with the possibility of intelli-
gent technology selection mechanisms based on improved situational
awareness.

_3.3. Dataprocessing_

Wearable-based data are gathered and processed in large quantities
depending on the individual product, yet it is always similar at its core.
Fig. 6 depicts the basic cycle of wearable data. The individual stages of
wearable data processing are characterized below before the details on
the data transmission aspects.

_3.3.1. Datacollection_
Wearable devices primarily collect and process user-generated data,
and collective data collection is commonly referred to as crowdsourc-
ing, a powerful tool for collaboratively retrieving a large amount of
data. Crowdsensing is a way to enable the coordinated data gathering
from the devices. There are three standard sensing techniques [180].

- _Participatory (active) sensing_ refers to obtaining information
    through the user’s action, such as measuring one’s exercise on
    their smartwatch.
       - _Opportunistic (passive) sensing_ describes periodic action to gather
          information, determined by elapsed time, distance, or other met-
          rics from the last data gathering.
       - _Opportunisticmobilesocialnetworks_ refer to self-organizing, point-
          to-point networks of devices sharing the information between
          themselves. The devices create the networks based on the vicinity
          to each other. Such networks can additionally assist other func-
          tions of the wearable, including positioning or user protection.

```
3.3.2. Pre-processing
Even though the central part of data processing takes place in
different computing layers [181], sometimes minor filtering processes
are executed in wearable and IoT devices. The early pre-processing
stage is essential for wearable and IoT devices since they do not have
enough computational and storage resources to process ‘‘unnecessary’’
data.
It is essential to highlight that the collected data contain incomplete
and duplicate information, errors, inconsistencies, etc. It requires an
early preparation before the data processing (locally or in the Cloud).
Thus, once the data is collected, it should be filtered, structured,
cleaned, and validated to improve the data’s quality. As a result, the
data processing step will take less time, and the output information
will deliver better decisions.
During the data preparation, some steps take place to enhance
the data and avoid unnecessary processing. For instance, gathering
information is devoted to finding the most ‘‘representative’’ data from
the collected set. It will be used throughout all the data processing.
The cleaning and validation are then essential to detect the quality
issues, including duplicate values, outliers, missing values, and incon-
sistencies. Once these issues are detected, multiple techniques can be
used to remove missing values, delete outlier samples, merge duplicate
data, etc.
```
```
3.3.3. Datatransfer
The data transfer phase is an essential part of the wearable device
data chain, and it is further discussed in detail in Section 3.4. At this
point, we only note that many wearable solutions limit the amount
of power spent during the data transmission by pre-processing it to
decrease the actual amount. For example, it is achieved by applying
compression schemes to the data before transmission [37]. Addition-
ally, the power constraints usually limit the transmission’s security, as
proper data encryption is often computationally demanding.
```
```
3.3.4. Computingparadigms
Based on architectural development, it is reasonably straightforward
to understand the specifics of wearable data processing. Computation
and operation on bulky and raw data was a challenging task. Thus,
during the firsts steps of the architectural evolution, wearables were
mainly utilized as data collectors. For example, ECG monitors were
given to patients for a few days to collect the data on the heart’s
rhythm and electrical activity. After that, the devices were connected
to a personal computer with a wire for post-processing. This phase
could be treated as the introduction of Multi-Access Edge Computing
(formely Mobile Edge Computing) (MEC) for wearables, i.e., moving
heavy computations to the closes network device instead of local
computations.
With the smartphone’s introduction as a gateway, wearable data
processing on it was adopted swiftly. Following the vendors’ foot-
prints, most application developers aimed to save battery-constrained
wearable lifetime by moving the smartphones’ computations. The Edge
operation hardened. Simultaneously, some AR/VR devices still do not
have the required processing power or tend to overheat. Thus, the only
option is to utilize a powerful Edge device for computing in trade-off
to transmission overheads.
Today, wearable devices mainly follow Edge and Cloud computing
paradigms, as well as Fog Computing [182,183]. The latter one is
```

```
Computer Networks 193 (2021) 108074
```
coined by CISCO in [184,185] and bridges the gap between the cloud
and end-devices, allowing the computation, storing, networking, and
data management near the target computationally-weak devices. In
contrast to Edge computing, which handles data on a nearest network
Edge node, Fog Computing processes data on a more powerful Fog node
in a more general way, i.e., to equip the network Edge and network
devices with virtualized services in terms of processing and storage
along with offering network services. To this end, the Fog found little
integration on wearables due to their proprietary communications/-
computing nature and lack of knowledge about the devices in proximity
and related communication aspects.
Cloud, Fog, and Edge computing are three levels that simplify
IoWT. Nevertheless, there are many more paradigms suitable for the
integration with wearables in reality [186], and the whole cloud system
is much broader and more complex [187]. The actual classification
also covers Mist Computing, Mobile Computing, Mobile Cloud Com-
puting, Mobile ad hoc Cloud Computing, Multi-access Edge Comput-
ing, Cloudlet Computing, and Transparent Computing [188]. In this
section, we overview these paradigms and explain their peculiarities
from the wearable technology perspective, whereas the implementation
challenges of computing paradigms will be discussed later in Section 4.

- _Mist Computing_ is operating at the Edge of the network, usually
    consisting of energy-constrained microcontrollers and sensors. It
    is a network without data processing. In this case, the data is
    generated where it interacts with the physical world.
- _Mobile Computing_ is a technology that allows transferring data,
    voice, and video through a computer or any other wireless de-
    vice (e.g., wearable, mobile phone, laptop, tablets). Mobile com-
    puting is used to create context-sensitive applications (e.g.,
    location-based reminders).
- _MobileCloudComputing_ is a platform that brings together mobile
    devices and cloud computing and creates an infrastructure where
    both data storage and processing take place outside of a wearable
    device. It allows accessing the cloud remotely using a mobile
    device.
- _MobileadhocCloudComputing_ refers to a group of mobile (wear-
    able) devices in the proximity willing to share their resources,
    taking some incentives and collectively solving the task. It is
    usually deployed over mobile ad hoc networks and performs
    computation-intensive applications using other portable devices’
    resources in specific scenarios, such as natural disasters, sports
    broadcasts, etc.
- _Multi-access Edge Computing_ (formerly Mobile Edge Computing)
    pushes the boundaries of Edge Computing by providing com-
    puting and storage resources next to low-power, low-resource
    mobile devices. It ensures connectivity and computing opportu-
    nities through wireless networks. In contrast, Edge Computing
    works solely between the mobile device and the closest powerful
    network node. This computing paradigm could be defined as an
    enabler for future wearable systems.
- _Cloudlet Computing_ is an infrastructure that uses small data cen-
    ters to move the functionality of the main data centers and
    bring the cloud closer to service consumers (being, essentially,
    wearables) [189]. Cloudlets represent virtual machine infrastruc-
    tures that operators place between devices and the cloud. This
    paradigm is mainly focused on real-time applications for resource-
    constrained devices.

Indeed, the variety of options to efficiently execute computing
between mobile nodes is vast.

_3.3.5. Dataprocessing_
During the data processing phase, different techniques and methods
are applied to the input data to obtain meaningful information. Nowa-
days, ML techniques are broadly applied to analyze and process the

```
data, such as clustering, regression, classification, among others [190].
Additionally, these ML techniques can be run by using batch process-
ing [191], real-time processing [192], and online processing [193].
Generally, the most significant part of the data collected by wear-
ables are time series [194]. This kind of data could be typically used
for classification purposes, anomaly detection, or forecasting. How-
ever, there are few obstacles connected to the analysis of time series.
The main one is the limited amount of data, which can be dealt
with using data augmentation techniques. The other issues are limited
computation capacity together with limited power resources when the
computations need to be done directly on the hardware.
Additionally, in the case of time series, other aspects should be con-
sidered, such as the occurrence of class imbalance and the possibility of
multivariate time series. Unfortunately, the commonly applied method
of augmentation could not be transferred from the image and speech
domain into time series. This created demand to elaborate on the
augmentation method for time series data [195]. The categories of the
time series’ augmentation techniques include six domains, i.e., time do-
main, frequency domain, decomposition-based methods, model-based
methods, learning-based methods, and time–frequency domain.
The recorded time series gathered by wearables contain a special
pattern, which indicates, for example, human behavior or physiological
disturbances, potential pathologies. For creating a predictive model,
it is necessary to use special ML techniques. Nonetheless, the pre-
processing steps are also needed to obtain the final expected results.
In terms of architectural choices, Convolutional Neural Network (CNN),
Long Short-Term Memory (LSTM), Bidirectional Long Short-Term Mem-
ory (BLSTM), Multilayer Perceptron (MLP), Gated Recurrent Units
(GRU), and transfer learning are robust in obtaining the state-of-the-
art results for wearable data [196–199]. Additionally, the usage of
classifier XGBoost was registered for the scalars’ values [200]. How-
ever, it required earlier feature extraction steps. The LSTM and BLSTM
architectures are suitable for this purpose because they can learn the
long-term dependencies occurring in the signal [201,202]. 1D-CNN
allows the algorithm to extract features and learn in time series what
is expected for such purpose [203].
After the data processing stage, the useful information is exposed to
the user through reports, graphics, tables, etc. It is then available for
further storage, applications, and development.
```
```
3.3.6. Datastorage
In this last step of data preparation, the altered data is stored for
further analysis, which is then used by recommendation systems for
marketing purposes and collective intelligence to improve the decision-
making process.
```
```
3.4. Communicationtechnologies
```
```
The wide range of wearable devices and related technologies allows
for various supported connectivity solutions, defined by the wearable’s
requirements for range, data rate, power restrictions, mesh types, devel-
oper’s preferences, and numerous other aspects. Data transfer specifics,
including encryption level, coding and transmission schemes, modu-
lation, and cyclic prefix, are also individually defined depending on
the utilized technology. The most commonly used data transmission
technologies in wearables include Near Field Communication (NFC),
Bluetooth Low Energy (BLE), Wireless Fidelity (Wi-Fi), ZigBee, Low-
Power Wide Area Network (protocols) (LPWAN), and other cellular
or non-cellular IoT transmission technologies [204]. As illustrated in
Fig. 5, both short-range and long-range communication technologies
are being deployed in wearable networks. This subsection outlines
the related communication technologies already available on modern
wearables and promising candidates widely discussed to be integrated
into the devices.
```

```
Computer Networks 193 (2021) 108074
```
_3.4.1. Short-rangecommunicationtechnologies_
Generally, wearable devices can communicate with each other in
a Peer-to-Peer (P2P) manner and with the gateway nodes using short-
range technologies in mobile wearable networks.
Bluetooth (and its currently broadly adopted version BLE) is a
short-range communication protocol for Personal Area Network (PAN)
working at a maximum transmission distance of 100 m and the 2.4 GHz
unlicensed Industrial, Scientific, and Medical (ISM) band. A piconet
is the most straightforward pattern of a Bluetooth network, and it is
composed of the _master_ of the connection (commonly, a gateway node),
and a maximum of seven served active _slaves_ (clients) [205].
The second primary wireless short-range technology is defined by
the IEEE 802.11 standard, also known under the market name of
Wi-Fi, which aims to provide connectivity to mobile devices within
the Wireless Local Area Network (WLAN). A direct connection between
devices is allowed by the ad-hoc mode foreseen by the standard,
nonetheless, the lack of efficient power saving and enhanced Quality of
Service (QoS) has pushed the Wi-Fi Alliance to make a move towards
the Wi-Fi Direct option, which handles the P2P communications more
efficiently [206].
Moreover, the current development of AR, VR, and XR technologies
dictates the need for higher throughput and lower delays. Developers
are opting for technologies that operate in high and ultra-high fre-
quencies, e.g., Institute of Electrical and Electronics Engineers (IEEE)
802.11ad, IEEE 802.11ay, and IEEE 802.11ac that can provide Gigabit
data rates in millimeter-wave band (mmWave) [207]. Moreover, the
use of these high frequencies has its propagation limitations, which
is ultimately an advantage for dense packing scenarios, where human
bodies act as a natural barrier and allow better utilization of spatial
reuse [208,209].
The Terahertz (THz) frequency band ranging from 100 GHz to 10
THz offers substantial bandwidth, theoretically enabling capacity in the
order of terabits per second at negligible latency. The THz frequency
band has been experimentally utilized for communication purposes at
short and medium ranges [210]. Currently, the THz frequency band
is a subject of exploration for point-to-point communication among
regulators, operators, and manufacturers. Visible Light Communica-
tions (VLC) is among the connectivity solutions that operate in the THz
frequency range, more precisely from 400 and 800 THz ( 780 – 375 nm).
This technology can simultaneously achieve illumination and commu-
nication between two or more devices in proximity, thus improving
energy efficiency using existing lighting infrastructure [211].
The wearable communication technologies with the shortest range
correspond to Radio Frequency Identification (RFID)/NFC systems.
RFID nodes can be worn by workers to provide them with hands-
free operations and allow flexible and mobile asset tracking by being
attached to gloves, hats, or helmets [212], and operating on the same
13.56 MHz frequency [213].
More advanced opportunities are brought to wearables by long-
range technologies. In contrast to the short-range communication (with
short-range technologies enabling a longer battery life, cheaper and
less complex devices [214]), long-range ones eliminate the application
selection limit, and wearable devices can communicate directly with
an access point, a base station, or an edge node. As a result, some
companies provide solutions for wearable devices with the opportunity
for either physical or embedded subscriber identification module (SIM)
cards to integrate long-range technologies. These solutions include
models from Apple, Samsung, LG, and Xiaomi.

_3.4.2. Long-rangecommunicationtechnologies_
Motivated by the increased popularity of these solutions, 3GPP
introduced its Massive Machine Type Communications (mMTC) tech-
nologies for low-power operation and reduced-complexity devices,
namely Narrowband Internet of Things (NB-IoT) and Long Term Evolu-
tion (LTE)-M [179]. The introduction of these technologies paved the
way for the usage of cellular modems in standalone wearables. First

```
introduced in The 3rd Generation Partnership Project (3GPP) Release
13 specifications, both technologies are optimized to communicate
small amounts of infrequent data with minimal power consumption and
maximal coverage. Taking into consideration the traffic requirements
of wearable applications that might be higher in comparison with smart
city or other more common Low-Power Wide Area (LPWA) use cases,
several enhancements to the NB-IoT and LTE-M standards are suggested
in 3GPP Release 14 specifications to offer higher data rates while still
consuming less power.
Nonetheless, presently deployed in cities, LPWA technologies are
already utilized for cases of long-range communications and low energy
consumption requirements [215]. The first target of these technologies
was low-end IoT devices such as sensors. However, LPWA connectivity
solutions have started attracting other application scenarios used in
wearable systems. An example of non-lincensed LPWA technology is
Long Range LPWAN protocol (LoRa). It is a long-range wireless tech-
nology that operates in the license-free ISM radio band at 868 MHz and
offers transmissions up to 25 km operational distances. This technology
has been deployed mainly in e-Health applications, such as temperature
sensor-based wearable devices, to evaluate and predict heart failure
events in high-risk patients [216]. Another alternative LPWA technol-
ogy used by proprietary wearable devices is Sigfox, which, similarly
to LoRa, operates at the sub-GHz ISM band and provides extended
coverage. While LoRaWAN is based on a spread spectrum technology,
Sigfox is a narrowband technology owned by the Sigfox company in
charge of deploying their networks [217].
Table 3 provides additional technical details on the short-range and
long-range communication technologies that are deployed in wireless
networks for the support of wearable applications. It lists most modern
ISM-band technologies ranging from conventional Wi-Fi to Wireless
Gigabit Alliance (WiFi at 60 GHz) (WiGig) as well as paid-spectrum
ones. In summary of this section, despite the conventional operation of
wearable devices via relays, the next-generation wireless networks aim
to provide standalone wearables with the opportunity of establishing
direct communications with the cloud.
```
```
3.4.3. Device-to-Device(D2D)-basedcommunicationforwearables
Multiple works propose to support wearables through D2D commu-
nication to increase the wireless networks’ capacity and coverage by
enabling immediate communications between the users.
```
```
3.4.3.1. Task caching and offloading. The research community has ex-
tensively discussed the rapid growth in the amount of data and the
number of computations on wearable devices. For example, the au-
thors of [218,219] introduced a data-driven resource management
framework to perform service-aware resource allocation and improve
resource ratio utilization with D2D communications. More specifically,
real-time communications between virtual reality and other wearable
devices are based on Edge caching. In this scenario, using D2D tech-
nology improves the cache hit ratio by considering mobile caching
and small cell caching – Base Station (SBS). Besides, D2D communica-
tions increase wearable devices’ bandwidth in ultra-dense 5G and B5G
cellular networks.
Moreover, the researchers have sufficiently covered task offloading
strategies to minimize processing time and, therefore, save power for
wearable devices with low battery levels. The authors of [220] propose
using the D2D link to create mMTC and, thereby, overcome the limited
resources of mobile devices. A similar approach is used in [221],
where nearby wearable devices form a local mobile cloud and thus
provide low latency. In [222], Dust (prototype code uploading D2D)
uses Google Glass as a prototyping device and offloads tasks using
D2D and the cloud. The authors of [223] provide computational of-
floading recommendations for AR applications running on wearable
devices. In [224], the authors propose a data offload platform for
other nearby applications and emphasize that Wi-Fi Direct D2D binds
to maintain high data rates for locally linked groups compared to
```

```
Computer Networks 193 (2021) 108074
```
**Table 3**
Wireless technologies comparison for wearable communication.
Communication technology Topology Frequency bands Range Data rate Power profile

```
Short-range
```
```
RFID P2P 125–134 kHz,
13.56 MHz,
860–960 MHz
```
```
Up to 100 m Varies with frequency Very Low
```
```
NFC P2P 13.56 MHz < 0.2 m Up to 424 kbps Very Low
BLE (IEEE 802.15.1) P2P, mesh, star 2.4–2.48 GHz Up to 100 m Up to 24 Mbps Low
Zigbee (IEEE 802.15.4) P2P, mesh, star 868–868.6 MHz,
902–928 MHz,
2.4–2.49 GHz
```
```
Up to 100 m Varies with frequency Very Low
```
```
Wi-Fi (IEEE
802.11a/b/g/n)
```
```
D2D, mesh, star 2.4–2.48 GHz,
4.9–5.8 GHz
```
```
20-250 m 2-600 Mbps Medium
```
```
Wi-Fi 5 (IEEE 802.11ac) D2D, mesh, star 4.9–5.8 GHz Up to 70 m Up to 3.5 Gbps High
Wi-Fi 6 (IEEE 802.11ax) D2D, mesh, star 1–6 GHz Up to 120 m Up to 9.6 Gbps High
WiGig (IEEE 802.11ad/ay) D2D, mesh, star 57–70 GHz 10–100 m Up to 20 Gbps Very High
VLC (IEEE 802.15.7) D2D, mesh, star 400–800 THz Up to 100 m Varies with frequency Very High
```
```
Long-range
```
```
NB-IoT Star-of-star LTE frequency bands Up to 15 km Up to 250 kbps Low
LTE-M D2D, Star-of-star LTE frequency bands Up to 10 km Up to 1 Mbps Low
LoRa Star 867–869 MHz Up to 50 km 50 kbps Very Low
Sigfox Star 868–878.6 MHz Up to 50 km 100 bps Very Low
```
Bluetooth and BLE. The context-sensitive upload structure (to cloud or
smartphone) was developed in [225] to achieve a trade-off between
the usability of wearable devices and the energy savings on the smart-
phone. As a result, the power consumption of unimportant tasks and
the waiting time for urgent tasks are significantly reduced.

_3.4.3.2. Software-defined D2D communication._ To combat a problem
of computational constraints and other critical issues faced by wear-
able communications (see Section 4.7), the authors in [214] propose
multiple-layer communication architecture, which incorporates D2D
cloud/edge technologies, Software-Defined Networks (SDN),
Heterogeneous Cloud Radio Access Network (HC-RAN), Multiple Input
Multiple Output (MIMO), and mmWave technology, among others.
In [226], SDN architecture for supporting D2D communication between
nodes of Wireless Sensor Network (WSN) is proposed to maintain
connectivity even in the case of the cellular infrastructure failure or
when it becomes partially unavailable. The authors particularly exploit
D2D technology to build a mobile cloud and perform computational
tasks on nearby devices. In the event of a disaster, the SDN controller
selects a multi-hop routing path. Here, the Cluster Head (CH) on each
mobile cloud associates with other CHs using inband D2D to convey the
information of out of coverage devices to the other part of the network.
Further, SDN based multi-standard cognitive radio is studied in [227]
for heterogeneous wearable wireless networks. It can control, config-
ure, select, and decide on switching between multiple technologies
based on the specific requirements in D2D communications.

_3.4.3.3. Millimeterwave-basedD2Dcommunications._ Using the mmWave
link is a tempting approach to achieve high data rates in wearable net-
works [228,229]. Moreover, the industry recognizes the importance of
mmWave technology for high-quality wearable devices [230]. For ex-
ample, the IEEE 802.11 working group is looking at high-performance,
mmWave-based wearables in public places as a possible use case.
As pointed out in [231], mmWave is an ideal candidate for D2D in
very dense scenarios because it requires directional transmission to
overcome high path losses, which in turn reduces interference between
adjacent lines [232]. Meanwhile, D2D is also beneficial for mmWave
picocells due to its high attenuation, especially for users at the cell’s
edge. Open areas of research in mmWave D2D communications, such
as gaps in ML, channel modeling, D2D clustering techniques, green con-
nectivity, and user mobility in mmWave D2D networks, are discussed
in [233]. Another interesting topic is covered in [234], which discusses
relay selection in mmWave D2D with dynamic obstacles.

```
3.4.3.4. Social-awarecommunication. Beyond the conventional connec-
tivity and interaction between heterogeneous IoT and IoWT devices,
the concept of Social Internet of Things (SIoT) supports a plethora of
socially-driven collaborations among objects [235,236]. The synergy of
social networking and IoWT paradigms offers some benefits and allows
devices to socialize, collaborate, and establish group-communications
according to the relationships. For instance, SocialobjectRelationship in-
cludes conventional human social relationships (e.g., owners of devices
are friends on Facebook, Linkedin, etc.), Ownership object Relationship
brings together devices held by an owner, Co-Work Object Relation-
ship integrates objects that work together to provide service for a
common IoT application, Parental Object Relationship clusters objects
belonging to the same production batch, whereas Co-Location Object
Relationship combines devices in the same place. The concept of using
elements of social networks in IoT has attracted an unprecedented
amount of attention from the research community [237,238]. Not
surprisingly, most of the research contributions in this field focus
on devices and their owners, their particular aims and needs, and
trustworthiness.
An overview of the integration of social-awareness and D2D com-
munication is presented in [239]. More precisely, the authors offer
state-of-the-art, socially-driven D2D communications by analyzing re-
lay discovery and peer selection, communication mode selection, spec-
trum resource allocation, and management when social concepts are
applied to them. In [240], the authors focus on social-aware D2D
communications in 5G cellular networks using matching theory for
caching problems. The authors state that the combination of D2D
and content caching can considerably improve system performance.
The work [241] presents a trust-based solution, where reliability and
reputation of devices based on SIoT concept are used for effective
D2D enhanced cooperative content uploading in NB-IoT. In [242], D2D
communication is applied to acquire the context-aware information and
integrate it with networking information elaborated at BS for infor-
mation diffusion time estimation in the The Fifth Generation Cellular
Network Technology (5G) network. In [243], the authors combine the
Diffie-Hellman Key Exchange (DHKE) algorithm with the SIoT concept
to efficiently allocate network resources to reliable nodes. In [244],
a D2D-based group technique to operate in sensor network environ-
ments, which contains a vast amount of devices, is proposed. This
approach allows reducing data congestion and ensuring outstanding
power efficiency.
```

```
Computer Networks 193 (2021) 108074
```
_3.5. Localization_

In recent years, the importance of wearable devices in our daily
lives to provide location and tracking of users within an environment
and their interaction with the plethora of Location-Based Service (LBS)
has increased considerably. However, the wearables that perform these
features present performance limitations in some scenarios and appli-
cations. Therefore, researchers are developing new positioning systems
considering the latest wearable devices’ strengths and limitations to
counteract these limitations and increase the positioning performance.
These new solutions include the implementation of new technologies,
techniques, and methods.
Given the fast growth of wearable devices that use positioning
and localization services, it is common to find them equipped with
GNSS chips. Currently, GNSS-based navigation systems have about 158
satellites in orbit for positioning purposes.
Hence, some wearable devices can estimate the user’s position by
using GPS or other constellations. Some companies are implementing
new technologies to provide highly reliable positioning services in
wearable devices. For instance, in order to reduce the power consump-
tion, Sony Corporation will incorporate a GNSS receiver in low profile
devices when dual-frequency is used to compute the user or device
position [245].
We can distinguish two main classes of positioning systems based on
the main wearable architectures: infrastructure-based and
infrastructure-less [246]. On the one hand, infrastructure-based sys-
tems are those systems that depend on a specific infrastructure to
estimate the position. The infrastructure can be deployed exclusively
for the system or be part of another system designed for a different
purpose [247,248]. On the other hand, infrastructure-less systems work
without requiring any surrounding infrastructure [249,250].
With respect to the application environment, wearable positioning
systems are classified as indoor and outdoor positioning systems. In
indoor environments, applications demand high accuracy position com-
pared to those used outdoors [251]. Additionally, each environment
presents particular challenges for positioning systems, for example,
the occlusion of view of the skies due to ceiling and signal multi-
path due to the complex geometry of indoor environments. Therefore,
depending on the type of environment, the positioning technologies
and techniques implemented are diverse to face the environmental
conditions [252].
In outdoor wearable positioning, the Global Positioning System
(GPS) and the cellular networks are the most used technologies [252,
253]. Regarding cellular networks, in each of their generations, the po-
sitioning accuracy is improved. Since the second to the fifth generation,
the actions carried out to improve the positioning accuracy are: use
the cell-ID localization technique, timing via synchronization signal,
specific reference signal designed for localization, and using all the
layers of protocol stack [254]. The technologies most used for indoor
positioning are: BLE, Wi-Fi, RFID, NFC, Ultra-Wide Band (UWB), Light,
Computer Vision, Magnetic Field, Sound, Dead Reckoning, and Tactile
Odometer [255].
In addition to traditional positioning systems, more complex sys-
tems have been proposed to enhance positioning accuracy and perfor-
mance. For example, Collaborative Positioning Systems utilize neigh-
boring wearables/users in the positioning system method, and systems
based on sensor fusion combine diverse sensor information to reduce
the estimation error of position [256].
Localization can significantly enhance the capabilities of wearables.
For instance, it can help users navigate and provide clues to devices
about interacting with users based on their location. Besides, location
services play a crucial role in emerging fields such as assisted living,
smart homes, and smart cities. Thus, the recent Location-Based Service
(LBS) must be compliant with the current legislation in terms of privacy
and security [257].

```
To summarize, choosing a suitable localization technology depends
on the application requirements. Table 4 compares some of the most
popular wireless technologies that can be used in the localization of
wearables. Some technologies are already present in wearables (GPS,
Wi-Fi, or BLE) but have accuracy in the range ofdmtom. UWB and
RFID-based localization technologies are relatively accurate but are
infrastructure-based.
```
```
3.6. Interoperability
```
```
The integration of multiple subsystems is the basis for modern IoT
and IoWT systems. However, it generates new interoperability prob-
lems and requires additional attention from the industry and research
communities to create seamless programmability of the various things
to connect, collaborate, and effectively exchange the data among
them [277]. Moreover, interoperability faces diverse challenges under
different scenarios in various fields and domains.
Different factors can trigger interoperability issue [278]. For in-
stance, integration between different manufacturers, limited communi-
cation between different transport protocols, and no established rules
or standards at the application level can prevent seamless integration.
In this context, it is essential to manage the intrinsic heterogeneity
of IoT systems and provide effective solutions for seamless interoper-
ability among smart devices, sensors, etc. Accordingly, interoperability
is investigated from various perspectives, including device, technology,
network, syntactic, semantic, and platform [279].
```
```
3.6.1. Deviceinteroperability
IoWT is composed of a wide variety of smart objects or things
ranging from high-end to low-end devices. The former have sufficient
resources and computational capabilities, whereas the latter type of
devices is generally resource-constrained. However, the devices, which
are different in terms of computational capabilities and use differ-
ent communication technologies, may need to exchange information.
This challenges interoperability among various types of heterogeneous
devices of the IoT ecosystem. Device interoperability is related to
the data exchange between heterogeneous devices and communication
protocols and the possibility of integrating new devices into any IoWT
platform [279].
```
```
3.6.2. Networkinteroperability
The integration of the IoT heterogeneous systems requires interop-
erability at various protocol levels to work together [278] seamlessly.
This interoperability type deals with mechanisms that enable seam-
less, ubiquitous connectivity. To truly ensure network interoperability,
each system must be able to provide the data exchange with other
systems over different networks by focusing on such network lay-
ers functions as addressing, routing, mobility, security, and resource
optimization [280].
```
```
3.6.3. Syntacticinteroperability
As mentioned above, interoperability reflects the ability to exchange
information transmitted between systems in the form of messages. In
this context, a message can be studied on the syntactic level, where
its internal properties are considered. Syntactic interoperability refers
to the interaction of format and data structure used in any exchange
between the IoT heterogeneous objects and can be reached through
defined data and interface formats and encodings [277].
```

```
Computer Networks 193 (2021) 108074
```
**Table 4**
Comparison of localization technologies for wearables.
Technology Refs. Accuracy Maximum
range

```
Power
consumption
```
```
Localization
approach used
```
```
Advantages Disadvantages
```
```
GNSS (GPS) [258,259] 10 cm Global,
outdoors
```
```
0. 5 – 2. 5 W Time-based Global, widely-available. Only outdoors, low accuracy,
high power consumption.
Wi-Fi [246,260–262] dm- or
m-level
```
```
250 moutdoors,
50 mindoors
```
```
< 1 W Fingerprinting,
AOA, TOA
```
```
Widely-available, low-cost, often
does not need dedicated
infrastructure.
```
```
Good-accuracy localization
methods based on fingerprinting
require extensive training,
relatively low accuracy.
UWB [263–265] Order ofcm 300 m 100 – 500 mW TOA, AOA High accuracy and precision,
moderate costs.
```
```
Not widely-available (yet), needs
dedicated infrastructure.
BLE [266,267] Order ofm 100 m < 50 mW Fingerprinting,
TOA
```
```
Widely-available, ultra-low-power,
protocol stack suitable for the
IoT.
```
```
Low accuracy.
```
```
Non-visible
light
```
```
[268] Sub-mm 10 m N/A TOA Very high accuracy. Requires LOS, expensive.
```
```
Visible light [269,270] cm- or
dm-level
```
```
1. 4 km N/A TOA Can use ambient light sensors
commonly available in
smartphones.
```
```
Requires Line-of-Sight (LOS),
high-accuracy solution requires
dedicated hardware.
LoRa [271,272] m-level 20 km < 100 mW AOA, RSS Ultra-low-power, low-cost,
long-range, designed for the IoT
and sensor networks.
```
```
Low accuracy.
```
```
RFID (passive) [273,274] cm-level 15 m – AOA, POA Ultra-low-power, low-cost,
high-accuracy.
```
```
Expensive infrastructure, small
coverage area.
RFID (active) [125,275,276] m-level 150 m < 100 mW RSS Low-cost, medium range. Moderate accuracy, need to be
powered.
```
_3.6.4. Semanticinteroperability_
The need for semantic interoperability emerges when heteroge-
neous devices use different syntax to encode and decode their in-
formation [281]. For instance, reliable communication between the
source and gateway devices can be interrupted if a sink device fails to
decode a source data format into an understandable form. In addition to
the fact that the data generated by wearables may have defined data
formats, the data models and schemes exploited by different sources
are usually dissimilar and not always compatible [279]. Further, the
data may consist of different information and be represented in other
measurement units. This semantic incompatibility between the data
and information models leads to IoWT systems’ failure to dynamically
and automatically inter-operate (as they have different descriptions
or understandings of resources and operational procedures [282]). To
this aim, semantic interoperability enables different agents, services,
and applications to exchange information, data, and knowledge in a
meaningful way, on and off the Web.

_3.6.5. Platforminteroperability_
Platform interoperability issues arise in IoWT due to different oper-
ating systems, programming languages, data structures, architectures,
and mechanisms for things and data. The lack of platform interoperabil-
ity can lead to the inability to connect IoWT devices to heterogeneous
platforms, developing applications that use multiple platforms, and
delaying the implementation of IoWT technologies on a large scale. In
contrast, cross-platform interoperability will ensure broad collaboration
between platforms to offer the best solutions in different areas [283].
To this end, one may need to acquire comprehensive knowledge about
Application Programming Interface (API)s and information models of
platforms to adjust applications from different platforms [279].
Although IoT interoperability issues are addressed by several aca-
demic and industry studies, there is still no proper foundation that can
cover some related research issues discussed later in Section 4. The
lack of standards and the absence of cutting-edge technologies slow IoT
development. Therefore, interoperability is a challenge that needs to be
extensively studied to provide consolidated, reliable, secured, scalable,
and adaptable solutions for IoT networks. Seamless IoT device inter-
operability is believed to push and open the massive opportunity in
the IoT market, accelerate industry innovation, and help developers and
companies produce solutions quickly.

```
3.7. Massconsumerdirections
```
```
In this section, we first overview the main wearable development
activities happening in the industry and proceed with the literature
review on recent academic works in the area.
Generally, the wearable devices’ market is flooded with new so-
lutions developed at both the academic and industrial levels. This
subsection provides a vision of a variety of prototypes and research
directions present in the industry. The next subsection would give an
overview of the leading academic projects and activities. Note that this
subsection particularly focuses on projects that are not yet present on
the market. A detailed overview of ready-for-purchase devices (together
with prototypes) is given in Appendix.
Moreover, today’s mass-market of wearables is driven by corpo-
rations aiming to push the adoption of high-end wearables to cus-
tomers. For example, Samsung is the most prominent owner of wear-
able patents, counting 3421 [284] active ones. At the same time,
Samsung was the global leader in the number of granted patents in the
years 2010–2018, counting 796 [285] granted patents.
While focusing on other industrial giants together with Samsung (Mi-
crosoft, LG Electronics, Sony, Alphabet, Epson, Philips, BOSE, Apple,
and OPPO Electronics), their intellectual property concerns more than
50% wearables. Therefore, more applications of market-available wear-
ables include monitoring of disabilities, education, enterprise, finance,
gaming, and entertainment. In general, the Asia–Pacific market is the
most active in the world in this area.
```
```
3.7.1. EntertainmentandAR/VR/XR
Concerning entertainment, another fast pacing wearable market
niche is related to VR devices. The adoption of said technology was
previously limited by hardware and communication issues, i.e., low
computational power and high bandwidth that were not reachable with
conventional wireless systems. Today, several VR headsets could be
purchased with reliable wireless connectivity while keeping the user
experience on a high level [208].
Companies are also integrating positioning and heading into their
state-of-the-art devices. A clear example is Sony, which is developing
a HMD. The contents on the HMD are adjusted depending on the user’s
pose and position to provide a full augmented reality experience for
```

```
Computer Networks 193 (2021) 108074
```
gaming on other applications [286]. Thus, the position and heading are
essential, but the head tilt is needed to re-allocate the elements on the
screen. Although the positioning techniques are well-known and most
of their problems are already solved, they face the restriction of energy
consumption imposed by the gadget size. Therefore, their efforts are
dedicated to the efficient combination of all the available sensors, as
demonstrated in [287].
Another area of interest includes Industrial Internet of Things (IIoT)
field. In particular, RealWear company focused on products specifically
designed for connected enterprise employees to increase job satisfac-
tion, productivity, and, most importantly, safety [288]. The company
has been developing an industrial hands-free portable computer for
many years, aiming to improve the employee’s situational awareness,
providing vital information on demand in the harshest conditions.
Today’s technology combines a small Android computer and a camera,
speaker, and microphone in a tiny screen project information in front
of the user’s eyes. This rugged hard hat is an intelligent headset that
works similarly to the original Google Glass but uses the underlying
technology in a completely different way.
Another project called Kopin Golden-i Infinity is also designed to
improve workers’ life with AR technology [289]. The device is used to
understand better the repair guidelines for field maintenance, access
to production plans, view utility, and energy information, collaborate
with remote experts, and more. Besides, the device boasts a nine-axis
stabilization head, triaxial accelerometer, gyroscope, and magnetome-
ter. This sophisticated tracking system evaluates the effect of the Earth’s
magnetic field on the user’s geographic position and head movement,
providing unprecedented tracking accuracy for applications requiring
incredible accuracy. Kopin also develops medical AR glasses for surgery
purposes [290].
Nonetheless, Nsoft and Trimble made a hard hat with Microsoft
HoloLens XR headset built-in specifically for industrial workers [291].
The XR10 is a customizable helmet with an integrated rotatable
HoloLens 2 lens that allows construction work to be visualized on site.
This first partnership is a clear sign of where Microsoft hopes to go
with its second-generation headset, taking the technology outside of
the office to real-world sites.
Keeping AR and VR headsets as a standalone solution is a trend for
heavy machinery, crate, drivers, and maintenance employees that do
not require constant mobility. However, complex computation on head-
mounted devices is still challenging due to battery and computation
limitations and overheating issues. Company Zebra produces portable
computers aiming to overcome those issues [292] and potentially of-
fload the computations to powerful yet portable wearable cloud nodes.
Complete Zebra solutions are based on Android enterprise devices
delivering unrivaled scan performance and manageability. Zebra’s fully
wearable solutions combine mobile with wearable technology and
ease of pairing features providing the operational flexibility needed to
exchange complexity for productivity.
Started with Google Glass, many companies aim to develop personal
AR-based assistants. One of those is the well-known Vuzix [293],
which aims to develop next-generation AR smartglasses using Mi-
croLED Technology with the primary goal of miniaturization of the
integrated screen.
Interestingly, Tesla files a patent for Google Glass-like AR system
for faster, accurate vehicle production [294]. According to the patent
application, the technology uses computer vision to recognize objects
based on the object’s colors displayed on the camera view and the
device’s location. The recognized object is then compared with the
3D model library’s corresponding model and overlaid on top of the
digital data.
In contrast, Bose AR with audio provided an entirely new di-
mension of audio immersion by merging Bose AR technology with
sunglasses [295]. The device detects where the user’s location and
which direction the owner is facing via a nine-axis head motion sensor
and the GPS on tethered Android or iOS devices. The audio pumped

```
through the on-board headphones changes accordingly. A new wave
of head-mounted wearables is related to VR. During Mobile WOrld
Congress (MWC), Nreal Light smartglasses provide mixed reality for the
masses [296]
Indeed, enabling an enhanced immersion in other realities could
not be possible without easy-to-use assistance devices. One of those
is a haptic VR suit for industrial training. Brian Heater developed
by Valkyrie Industries [297]. Similarly to the Iron Man suite aims to
provide the ‘‘haptics is the sense of touch, particularly relating to the
perception and manipulation of objects using the senses of touch and
proprioception’’. Interestingly, the suite is designed not for gaming but
for professional applications, the list of which is kept untold.
```
```
3.7.2. Medicalandclose-to-medicaldevices
A massive sector is related to close-to-medial wearable devices,
i.e., ones that are not certified as medical ones but still aiming to detect
some health-related issues. For example, a French piece of technology,
Crhonolife smart vest, presented at the Consumer Electronics Show
(CES) 2019 event, aims to predict the heart-attack before it hap-
pens [298]. It is specifically designed to prevent medical emergencies in
patients with congestive heart failure (CHF). Some devices are designed
to monitor the owner’s posture, including Upright and Lumo Lift [299].
Many companies, including POLAR, Garmin, Fitbit, and others [300],
allow for heart rate monitoring but often do not focus on Food and
Drug Administration (FDA) approval.
On the other hand, some medical wearable devices have also suc-
ceeded in receiving FDA approval, including the well-known Apple
Watch [301] for the detection of falls and irregular heart rhythm,
thus, achieving Steve Jobs’ goal. Nonetheless, SYNCHRONY and SYN-
CHRONY 2 cochlear implants have also received the approval for peo-
ple with single-sided deafness (SSD) and those with Asymmetric Hear-
ing Loss (AHL) [302]. Next, Neofect’s powered glove for people with
paralysis is shipping this summer [148]. It provides the users with mo-
bility in a paralyzed hand (potentially present due to stroke, Multiple
Sclerosis (MS), and Amyotrophic Lateral Sclerosis (ALS). It allows
performing simple everyday tasks such as brushing their teeth, opening
doors, or drinking from a cup.
Another active niche of wearable industrial research leads to an ar-
tificial nervous system [303]. Researchers from NUS Materials Science
and Engineering developed the touch equivalent to human skin with
the Asynchronous Coded Electronic Skin (ACES). It can assist future
robotics in terms of providing sensual feedback for tactile feedback in
prosthetics.
A lot of research activity is currently executed related to Parkinson’s
disease. Based in Austria, EVER Pharma recently received CE Mark
approval and is releasing its D-mine Pump in Europe [304].
Patents have also shown the trends for medical wearables. In [305],
the authors introduce a wearable device integrated into a partial or full
body soldier’s garment, able to deliver wound sealant to an injury and
activate selective small balloon inflation to add pressure to a wound.
An alternative use-case considers its usage to stabilize the injured while
being transported.
Honda Motors patented a method to support the vehicle con-
trol [306]. The wearable devices can capture diverse physiological data
to determine one or more vehicle occupants’ health state. These data,
such as the blood rate pattern, can also be used to identify a vehicle
occupant. Their method includes the total or partial control of the
vehicle based on its occupants’ health state.
```
```
3.7.3. Fashionandcomfort
A massive niche is allocated to the mass consumer by means of
improving the comfort of everyday activity and fashionable look. The
number of devices ranges a lot, from luxury smart rings to invisible
personal assistants.
An exciting segment of wearables is novel wearable air conditioning
systems. To name a few, Sony Reon Rocket is a body-cooling wearable
```

```
Computer Networks 193 (2021) 108074
```
that promises to chill the owner in the heat [307]. Sony is not the only
company attempting to capitalize on the rising heat. Embr Labs is a
startup founded by three MIT graduate students who were frustrated
that it was always freezing in their lab in the summer, even when there
are only a few people in the building [308].

_3.7.4. Consumersports_
Besides the conventional market segment of activity trackers and
smartwatches, few more vendors focus on the development for a spe-
cific group of users — athletes aiming to improve their results utilizing
better monitoring and improved training [309]. Catapult [310] and
STATSports [311] are trendy suppliers of wearables to the top sports
teams in soccer, football, hockey, rugby, and baseball. These producers
offer small devices worn in the special vest pockets on the back and
can perform indoor and outdoor localization and track the heart rate.
Specially developed software performs analysis based on collected data
and allows to manage workloads, monitor athlete progress, and avoid
situations that could lead to injury.
The authors in [312] introduced a wearable device used to record
fishing data. The wearable can receive motion data from one or more
motion sensors. Collected motion data is analyzed to determine if it
corresponds to a casting motion while fishing. In such a case, the cast
occurrence is recorded and timestamped.
Xsens [313] developed a real-time motion capture system named
MVN Analyze, which allows accurate tracking and analysis of the
athletes’ movements even during high-intensity activity. The system
is available in two versions: 17 wireless sensor straps (MVN Awinda)
or a Lycra suit (MWN Link) — both comfortable for the user and not
restricting his movement.
Another promising niche is related to the growing vehicular mar-
ket [314,315]. In particular, wearable devices may be used to assist in
continuous passenger biometrics monitoring during the autonomous ve-
hicle operation, thus, improving the overall safety of the system [316].
These include authentication while accessing the vehicle, passenger
presence, driver’s biometric status, sleep monitoring, etc.

_3.7.5. Security_
A sector with great research potential for wearables is related to
the information security domain. Already today, wearable devices may
enable safe transactions/payments on a mobile device based on a
wearable security token. It not only separates the security management
from the device performing the transaction but also reduces the risk
of impersonation or relay attacks [317]. Similarly, other wearable
devices have been patented to, for instance, safely store encrypted
information, which is only sent to a pre-specified mobile terminal after
verification [318]. Some wearables combine biometrics and advanced
encryption to allow specific secured transactions with a counterpart
communication device/system [319].
However, wearables are not only used for secure monetary or infor-
mation storage/transactions. The authentication possibilities through
biometrically secured access may also be used to, e.g., automatically
manage other smart devices [320] or send alerts in response to critical
situations according to the wearer’s vital signs [321].

_3.7.6. Otherindustrialactivities_
Some smaller companies are involved in developing novel niche
solutions and creating new applications. The examples are wearables
for well-being. Relaxation is a part of wellness that corresponds to the
fashion and comfort segment of wearables. The Silentmode’s Power-
Mask is a relaxation mask that keeps records of heart rate variability,
as stated in [132]. The Dreamlight Zen meditation & sleep mask is a
product that uses lights and music to help users calming down and
restoring their vitality.
The possibility of wearable devices to sense and act has also found
applications in stimulating sensitive parts of the body and/or measure
signals. In the adult entertainment market, various wearables were

```
designed to induce sexual pleasure. Besides practical products, some
design and technological efforts have been made to separate the drive
means from the stimulation means, enabling a fully autonomous oper-
ation [322], or, even, to allow remote controlling [323]. Other bodies
and muscle stimulation applications are also explored, for instance, to
tackle incontinence [324].
```
```
3.7.7. Active(Inter-)nationalprojects
While industrial giants aim to occupy more significant shares of
the market and increase their revenues, the academic sector is mainly
focused on promising technologies and evaluating existing devices’
performance.
A number of the international EU H2020 research projects are
focused on wearable solutions both from the Hardware and the Soft-
ware domains. Some of the ongoing projects are as following: Wear-
able Electroactive Fabrics Integrated in Garments (WEAFING) [325],
Smart and Flexible Energy Supply Platform for Wearable Electron-
ics (Smart2Go) [326], Personalized Body Sensor Networks with Built-In
Intelligence for Real-Time Risk Assessment and Coaching of Ageing
workers, in all types of working and living environments (BIONIC) [327],
Real-time Analytics for the Internet of Sports (RAIS) [328]. Moreover,
more than 400 projects related to wearables have received support only
from the EU since 2016.
From non-EU perspective, exceptional sense of touch for robots is
described in research [303,329]. As the device is called, ACES has a
somatosensory perception, which identifies a touch 1,000 times faster
than humans’ nervous system. A potential application for this technol-
ogy will allow performing critical surgery with better responses and
taking relevant actions in limited time slots.
Another project, described in [330], refers to the approach where
scientists present ultrasoft electronics as a concept for Body Area Net-
work (BAN). The researchers in [331] have developed a sample of heart
cells with a soft sensor and changed the way of embedded medical
devices.
The work described in [332] claims to create Magnetic Resonance
Imaging (MRI) detectors that fit like a glove. The developed solution
covers the situations where the hand moves in the magnetic resonance
scanner without degrading the signal quality, thanks to the MRI de-
tectors that seamlessly follow the contours of the hand using separate
flexible high impedance elements.
The activity in [333] presents a novel approach to using the NFC
technology to extract valuable knowledge from sweat analysis. This
study proves to cover a gap as a non-invasive solution working on
advancing the deployed sensors’ form factor. Another study in [334]
focuses on sweat analysis and claims wearables could analyze the data
to get more insightful information regarding the user’s physical and
mental state for improving the quality of training.
Overall, it can be stated that financial agencies are interested in
investing research funding in wearable technology research activities.
Interestingly, those are not anymore limited to eHealth and medical
domains, thus, allowing to cover activities in other fields.
```
```
3.8. Sectionsummary
```
```
This section outlined the classification of wearable devices based
on, e.g., location on the body, application type, functionality, etc.
It highlighted the communication technologies, architectures, and re-
lated paradigms, including technical details, elaborated on various
data processing-related aspects, and involved computing paradigms,
outlined localization strategies for indoor and outdoor operation, and
provided insight into the interoperability aspects, and, finally, delved
into the mass consumer market status. Additional information on the
devices is detailed in Appendix.
```

```
Computer Networks 193 (2021) 108074
```
**4. Open challenges and future perspective**

This section outlines the majority of modern problems related to
wearable data processing, privacy, security, and transmission aspects.
Next, localization and communication-related challenges are drawn,
followed by the adoption, hardware constraints, interoperability, and
scalability aspects.

_4.1. Dataacquisitionandprocessing_

A large part of the data acquisition challenges is in the first com-
ponent of the data processing chain, namely the wearable itself. The
quality, quantity, resolution, and other parameters of the data are
defined there. As crowdsourcing gathers data from multiple users,
multiple devices, all in different scenarios and often using relatively
cheap and energy-efficient sensors, the quality of the data itself can
enormously vary across all individual data sources [335]. The quality
and quantity can be related to spatial resolution, temporal resolution,
or data resolution itself [160]. Spatial resolution determines the phys-
ical distance between two consecutive measurements from a single
source and can be equidistant or strongly varying. Temporal resolution
describes the time intervals between the two measurements from a
single user and can be uniformly distributed or strongly randomized.
The data resolution relates to the accuracy of the measurement sensors
equipped in the user wearable, device-specific processing inside that
wearable, and outside factors affecting the measurement itself.
The subsequent challenge lies in the large-scale data gathering pro-
cess, i.e., finding the optimal method of gathering the users’ measure-
ments for further utilization [336] and its energy-efficient transmission.
The question of privacy, security, trustworthiness, or user selection is
nowadays still an open challenge [337].
Data processing challenges also describe the difficulties in data uti-
lization after the acquisition phase. As mentioned above, the data have
different spatial and temporal resolutions and varying data quality.
Converting raw, gathered data into useful data is the main task of data
pre-processing. The challenge lies in unifying the measured quantities’
parameters and removing errors and statistical outliers from the data.
Further data analytics require a clean input dataset and represent a con-
secutive challenge itself. The efficiency of the analytics determines the
amount of useful information extrapolated from the set of individual
measurements. Nowadays, wearable-related data processing solutions
utilize machine learning techniques more often [338,339].
One of the main challenges of wearable data processing is the
lack of a sufficient amount of data. To overcome this issue, a few
categories of the time series data augmentation were proposed [195].
One of them is the augmentation in the time–frequency domain with
wavelet transforms as one of the potential successors in augmentation
of non-stationary time series and non-Gaussian noises [195]. More-
over, the combination of augmentation methods dedicated to imbal-
anced datasets from the used architectures weighting is also proposed
in [195]. However, using data augmentation methodology brings po-
tential problems, such as not reflecting the real data and possible
overfitting.
Next, the lack of etiquette of the data states an extra problem
because of the limited number of available datasets. Additionally,
obtaining high-quality labels is time-consuming and often requires
specialists for this purpose or engagement of the users [340,341]. One
solution is to use a semi-supervised methodology when the number of
the annotated labels is small. It could primarily be applied for the data
gathered by sensors and wearable devices with long records, e.g., the
Human Activity Recognition (HAR) task when not all the labels are
correctly reported by the users or labeled by the specialists [341]. These
same semi-supervised methods minimize the obstacles connected to
training the data lacking in labels.
HAR was successfully used in temporal assembling of deep
LSTM [342], LabelForest [343] or bi-view semi-supervised learning

```
method [344] leading to the understanding that it may be a promising
solution for classification tasks based on wearable data. Additionally,
combining many modalities for detecting diseases allows decision sup-
port methodologies for achieving higher quality results in prediction.
The limited number of works leaves a huge research gap, leaving ample
opportunity for future directions. The multimodal approaches were
used mainly hitherto for the human activity recognition [39], Parkinson
detection [345], difficulty in cardiorespiration [156].
A new trend of wearable technology for data gathering becomes
possible with the development of smart tattoos constructed from thin-
film polymers, metals, ceramics, 2D materials, and their integration
with rigid ICT [346]. Part of the smart tattoos will serve for the biomed-
ical tasks, i.e., gathering physiological parameters in real-time [347,
348], e.g., the genetically programmed cells could be transferred into
wearable devices.
Interestingly, smart tattoos were designed by Nokia as Vibrating
Tattoos, which are placed on the skin. They contain ferromagnetic ink
and vibrate when someone is texting or the mobile phone is calling.
Princeton and Tufts University developed the next unique smart tattoo
to measure bacteria levels in the mouth based on saliva with electronic
wireless tattoo [346].
Additionally, recent micro- and nanotechnology developments sup-
port non-invasive biomedical measurements and wearable in-body and
on-body sensing, processing, and communication. Examples of existing
solutions are insertable cardiac monitors, continuous glucose monitors,
Insertable Drug Deliverables Systems (IDDS). Shortly, the development
of the analyte monitors is being expected (for example, for monitoring
the oxygen concentration in interstitial fluid), insertable EEG moni-
tors (dedicated mainly for epileptic patients), eye health monitors (for
glaucoma patients). The most promising solutions are controlling the
infant, therapeutic drug monitoring, and delivery [124]. Furthermore,
the microneedle sensors’ usage will allow clinicians to monitor the
electrochemical parameters, for instance, measuring the level of lev-
odopa for Parkinson’s patients [349]. However, the main challenges
of the insertables belong, among others, the foreign body response,
which impedes the biosensors’ functioning, likewise the transmission
of the data or unexpected migration of the device [124]. One of the
approaches for reliable wearable platforms is to address the optimal
choices of sensors and user interfaces and conduct the validation of
methods based on the target application (e.g., clinical, social well-
being, etc.), data security and confidentiality, decision support, and
user acceptance.
Significantly, the eHealth segment is a strongly regulated sector
with high accuracy and reliability requirements. Mass-market wear-
ables’ accuracy cannot compete with often expensive hospital devices,
and currently, available consumer wearables are usually not acceptable
for medicine purposes. The reason is that wearable sensors often have
insufficient accuracy compared to laboratory devices. Another issue is
that devices from different production series can also suddenly measure
different values due to different electrical components, which in the
case of medicine can have serious consequences [350].
Crowdsensing data collection provides a significant advantage for
wearables over large and accurate laboratory sensors. It becomes an ef-
fective and low-cost approach for automatic multi-purpose data gather-
ing and processing [351]. Nowadays, it is commonly used, for instance,
to automatically generate radio maps or collect health parameters
for eHealth monitoring and activity recognition. Crowdsensing over
wearables has many unresolved challenges, which include data redun-
dancy and outliers’ identification and elimination, reducing the data
processing, transfer, and storage costs, leveraging the temporal and
spatial correlations of information to reduce the amounts of stored and
processed data, and dealing with heterogeneous devices and technolo-
gies [351]. Wearables can collect a variety of user-centric data, such
as location-related knowledge, information on the user’s well-being or
health [352], and radio communication-specific data.
```

```
Computer Networks 193 (2021) 108074
```
The development of the eHealth/mHealth field by applying wear-
able sensors is also of particular importance due to the rapid growth of
the elderly population in Europe. For example, monitoring the elderly
suffering from civilization or neurodegenerative diseases could allow
to detect of Parkinson’s or Alzheimer’s disease early and predict the
illnesses’ development [353].
Approximate computing is another technique that allows to trade
precision in exchange for increased energy and performance [354].
Many wearable applications, including ML, signal processing, image
processing, Big Data analysis, and more, may not require very accu-
rate results. Instead, results that are ‘‘good enough’’ can serve this
purpose [355]. Thus, approximation has become an effective method
for improving the performance and energy efficiency of devices with
limited resources, such as [356] wearables. However, this comes with
many issues, such as determining the minimum required accuracy,
defining approximate problems, and monitoring the results of the appli-
cation [357]. Hence, efficiently implemented approximation methods
can achieve optimal performance gains in latency, execution speed/-
time, and battery consumption.

_4.2. Datatransmissionaspects_

As we move towards a more connected ecosystem, data generation
will continue to increase, primarily due to 5G and beyond technologies
that ensure faster connectivity. However, not only technologies are
developing, but also the problems that surround them.
Although a centralized cloud has traditionally been used for data
management, processing, and storage, it has two major problems: (i)
the latency to process data may be critical; (ii) all this data creates
a significant load on the overall network performance. In contrast,
Edge computing offers a solution to latency by moving critical data
processing to the network’s Edge [358]. Edge devices can collect and
process data in real-time, allowing them to respond faster and more
efficiently. However, there are issues related to the devices’ capabilities,
including developing software and hardware to handle the cloud’s
computing load.
Different computing paradigms demonstrate great opportunities and
introduce new techniques to improve system performance. In practice,
computing paradigms are sometimes discussed as mutually exclusive
approaches to network infrastructure. Although they may function
differently, utilizing one of them does not preclude using the others.
In this context, some approaches have been proposed to solve this
issue (e.g., a cognitive IoT Gateways [359], a platform that automat-
ically determines the best environment to execute a task [360], and
a framework for scheduling applications over a hybrid public–private
cloud [361]). However, the automatic switching between computing
paradigms is a challenge for future research, in any case.
It brings the researchers to the problem related to the migration
of services or a Digital Twin (DT) of the wearable device, for in-
stance, from one Edge server to another [362,363]. When a user moves
across different geographical locations [364], e.g., from home to the
workplace, the service/DT may follow the user’s device. However,
the determination of an optimal migration decision is challenging
because of the trade-off between the migration and data transmission
costs [365]. On the one side, migrating a service/DT may incur net-
work overhead or even interrupt the connection. On the other side,
not relocating a service/DT may increase the data transmission delay
between the user and the edge server. In the literature, there are several
approaches to reduce the transmission delay in traditional wireless
communication networks concerning the migration procedure [366–
368]. However, ensuring seamless migration among Edge servers is still
an open problem that needs to be investigated.
Next, compressive sensing is gaining increasing popularity from the
lower layers perspective, especially for IoT applications that involve
sparse data signals. It is a signal acquisition and reconstruction tech-
nique that enables the receivers to reconstruct the actual signal using

```
significantly fewer samples than required by the Nyquist criteria. Com-
pressive sensing has proven to bring several benefits such as efficient
bandwidth and energy consumption, which are the two most vital
network resources in wearable networks [369,370].
```
```
4.3. Securityandprivacyaspects
```
```
In the previous subsection, we highlighted that wearable tech-
nology’s main features are sensing and collecting data continuously.
Therefore, with the advancement of the IoWT in next-generation cel-
lular networks, security and privacy are vital characteristics for con-
sideration in wireless communication scenarios [371]. Regarding the
widespread of modern data collection techniques and sensor develop-
ment, user concerns about reliability and trust in online platforms and
location-based services are continually growing. The authors of [372]
state that most modern devices include built-in sensors, which provide
accurate location data and information about physical activity level and
mental health. The study shows that the data is easily accessible and
does not correlate with users’ awareness. There is no unified solution to
cover all threats in wearable technology security. Thus, further research
and development are required.
```
```
4.3.1. Data-relatedaspects
In [392], the authors show concern about the actual owner of the
data collected via smart connected devices. Due to the proximity to
a human body, hereinafter, we claim wearable technology is one of
the most exposed wireless solutions to privacy threats. Privacy issues
are relevant to data integrity, and an attacker might physically affect
the owner via malicious hardware or software. As long as embedded
sensors in smart wearable devices crowdsource personal information
about technology users, data processing should be privacy policy com-
pliant. There are specific laws in countries worldwide that protect
the data privacy of their citizens. Currently, the primary document in
charge of data privacy and security protection in Europe is the General
Data Protection Regulation (GDPR) law. This document implements
newer focus areas, such as privacy rights, data security, data control,
and governance. Accordingly, all data collected via wearables can be
considered sensitive (e.g., genetic, biometric, and other health-related
data). Consequently, our survey provides a taxonomy for multiple
types of data that wearable devices are gathering via built-in sensors
in Table 5. As this survey investigates, the most popular solution to
exchange data on wearables is BLE, and many research experiments
report on its vulnerability to security attacks.
Evidently, in most of the security and privacy preservation scenar-
ios, it is necessary to perform complex cryptographic operations, which
are limited in wearables due to their low computing power and limited
resources.
```
```
4.3.2. Impactonenergyconsumption
The execution of the related complex operations implies, in most
cases, extra consumption of energy and resources, which considerably
reduces the duration of the battery. Despite the mitigation strategies
already discussed, these drawbacks mean that it would be an excellent
starting point to reduce the potential risk of future attacks. Their real
implementation on wearable devices becomes quite challenging. Today,
developers and researchers explore wearable technology’s security as-
pects, especially in the medical and industrial segments. The authors
of [393] investigated the executability of various primitives used in
symmetric and asymmetric cryptography, block ciphers, elliptic curve
cryptography, and conventional hash functions. The set of measure-
ments showed that the use of widely used methods leads to a significant
computational load on wearable devices compared to, for example,
smartphones. As one of the solutions, this work highlights the need to
develop specific lightweight primitives, taking into account the trade-
off between energy consumption and safety as one factor in creating
efficient devices with limited resources.
```

```
Computer Networks 193 (2021) 108074
```
**Table 5**
Taxonomy of sensors and data collected via wearable devices.
Sensor Biometrics Location Audio/Video Altitude Inclination Health data Other References
Gyroscope ✓✓ [373]
Accelerometer ✓ ✓ [373,374]
Altimeter ✓✓ [375]
Proximity sensor ✓ [376,377]
Temperature sensor ✓ [378]
Magnetometer ✓ ✓ [379]
IMU ✓✓ [380]
Camera ✓✓ ✓ [167,381]
Optical sensors ✓ ✓ [382,383]
Microphone ✓ [381]
Beacons ✓ [384]
Chemical sensors ✓ [385]
Antenna module ✓ [386,387]
Ambient light sensor ✓ ✓ [388]
NFC sensor ✓ ✓ [389]
Touch sensor ✓ [390,391]

_4.3.3. Privacyaspects_
Nonetheless, from Radio Access Network (RAN) perspective, several
entities can be considered to have access to the most sensitive data col-
lected by wearable devices. The actual device might be an adversary to
data integrity and security if not enough safety measures are considered
or no encryption has been used.
Since most of the wearable communications utilize D2D solutions,
i.e., when multiple devices are communicating in proximity (e.g., exe-
cute any collaborative tasks), securing those links became an essential
field of research [394]. D2D nodes in the proximity can share sensitive
information about the user identity and other personal data. As a
consequence, this personal information can be exploited for illegal
purposes by eavesdroppers [206]. Network security protocols in D2D
networks were developed to allow users to avoid any information leak-
ages. The major issue primary in secure D2D networks is the dynamic
readjustment required due to user mobility. Therefore, the need for an
adaptive mechanism for D2D network security emerges when the users
join or leave the coalition [395].
To conclude, although there has been a plethora of work related to
wearable architectures for efficient dynamic D2D communications, the
following topics are mostly missing in the literature: multi-connectivity
heterogeneous Radio Access Technology (RAT)s and mobility in the
IoWT, optimized link selection for highly dynamic multi-tenant net-
works, need for efficient privacy-preserving techniques, security issues,
the enhancements offered by a set of innovative 5G technologies in
practical IoWT contexts, among others. There are still no appropriate
communication architectures to converge wearable devices and net-
works with external Internet via the edge-computing infrastructures al-
lowing seamless and well-orchestrated integration and interoperability.
Therefore, multiple design choices and criteria need to be thoughtfully
studied in this field. For instance, the Inside-the-body (ITB) component
of the network could be connected to the user’s equipment (e.g., a
smartphone or high-end wearable device). These require real-time
access to the proximate edge cloud ecosystem, which offloads the
battery-constrained devices and processes their demanding computing
tasks remotely. This construction became even more challenging when
a user is on the move, and numerous technical challenges need to be
resolved in high dynamic scenarios.

_4.4. Localizationaspects_

Modern wearable technology heavily relies on the precision of
positioning techniques embedded in the devices. This subsection lists
the main challenges related to the localization of resource-constrained
wearable devices.
To start with, the geometry of indoor scenarios plays an essential
role in the robustness, precision, and accuracy of the positioning sys-
tems used on wearable devices. Mainly because the dominant position-
ing technology used by wearable devices relies on wireless technolo-
gies, e.g., BLE, Wi-Fi, UWB, with various signal propagation problems

```
being present due to the complexity and continually changing of indoor
environment [396]. Factors alter the signal propagation as propaga-
tion losses (e.g., reflection, diffraction, scattering), Non-Line-of-Sight
(NLOS), multipath propagation [396,397].
NLOS propagation radio signal is the primary source of the inaccu-
rate position, so mitigating its effects is one of the main challenges in
positioning [398–400]. A vast amount of methods for mitigating the
effects of NLOS on position accuracy has been proposed. For example,
the authors of [398] classify them into two categories, methods that
mitigate the NLOS into the positioning algorithm without previously
identifying NLOS and methods that implement a NLOS identification
phase first and then, in a second phase, mitigate the NLOS error from
the position estimation. In [401], the authors consider a cooperative po-
sitioning approach to address the NLOS estimation error issue. Despite
the great variety of methods proposed in the literature, the effects of
NLOS have not been completely mitigated. Crowded environments and
complex geometries scenarios still represent a challenge to overcome.
Finding a good trade-off between the accuracy and the energy
consumption of a localization system is an on-going challenge. In
particular, energy efficiency is a critical constraint of wearables due
to their small form factor and portability requirements, which prevent
them from using large batteries. While outdoors, the de facto local-
ization system for many wearables is GNSS, indoors there are many
competing technologies with varying degrees of localization accuracy
and energy efficiency. Widely-available technologies like Wi-Fi and
Bluetooth often rely on fluctuating Received Signal Strength (RSS)
measurements or imprecise Time-of-Arrival (TOA) estimates, which
decreases their localization accuracy. UWB-based localization systems
can achievecm- ordm-level accuracy and have a low energy consump-
tion. However, they are not readily available in most of the wearables
already on the market. Future efforts are required to develop accurate
localization techniques that can be implemented with low costs and low
overhead on small devices.
Location privacy is a major concern of wearable localization, as
location information in the hands of non-trustable parties can lead
to a disclosure of unwanted private information, identity theft, or
decreased safety. Communication privacy and authenticity validation
in wearables are also essential, as privacy suggests that an individual
keeps personal data as much as possible under control and to share
them only with ‘‘trusted’’ devices [402].
Building large-data collection platforms constitutes a Software (SW)
engineering challenge, which requires innovation in data analysis and
visualization techniques to gain insights into individual and aggregated
user patterns, i.e., Spatio-temporal clustering, visual analytics, etc.
Standardization is the most powerful framework to provide fast,
secure, and straightforward integration between different devices, com-
ponents, and systems. Various standards have not been fully adopted
```

```
Computer Networks 193 (2021) 108074
```
in existing localization systems, specifically in indoor localization plat-
forms. For instance, the authors in [403] evaluated indoor localiza-
tion systems and provided general comments on the International
Organization for Standardization (ISO)/International Electrotechnical
Commission (IEC) 18305 standard. The authors emphasized the lack
of standard evaluation procedures for the customized ILS and Indoor
Positioning System (IPS), impeding to be embraced in other environ-
ments. However, standardization is not only limited to the evaluation
procedures. It is also applicable to positioning technologies, indoor
maps, software communication protocols, devices, discovery protocols,
among many others.
The ISO/IEC 18305 [404] is an ISO standard devoted to identify and
define the most appropriate metrics and scenarios to assess localization
and tracking systems. Indeed, many researchers have reported difficul-
ties in comparing the methods with the published results because the
evaluation metrics reported differing in the literature (e.g., averaged
positioning error, mean squared error, median error, among others).
The experimental part and data collection in the literature present
significant differences with various evaluation area sizes and strategies
to evaluate the method, procedures, and protocols for data collection.
Thus, the ISO/IEC 18305 standards can be considered as a guide
on how evaluation results should be reported, including aspects on
the evaluation area, with special interest indoors. Additionally, some
initiatives standardize the evaluation of localization systems through
extensive sets of pre-collected data (datasets), providing an evalua-
tion framework that can be reproduced. Localization competitions are
also becoming popular in the evaluation as they allow the compar-
ison of real-time localization solutions under the same conditions in
challenging areas.
Although some of these standards are available in the literature,
most application platforms do not adapt to these standards. It results
in non-standards localization platforms that are difficult to integrate
with other systems, which is the major challenge for developing indoor
localization technology nowadays. As stated in [405], we need a com-
mon taxonomy with the related services and protocols, as it is the most
relevant missing piece in indoor localization now. The next steps should
focus on defining a taxonomy of ILS/IPS, outlining the framework to
allow the collaboration of multiple ILS/IPS, and drawing the required
standard services and applications in the near future.

_4.5. Communicationandarchitecturalaspects_

Smart wearables need to be interconnected in a heterogeneous
manner (i.e., different technologies and devices communicating with
each other), battery-operated. They may harvest energy, e.g., from the
sun or human motion. They enable various smart functions, which co-
operate in a decentralized manner and offer Internet access. Designing
efficient D2D-based capabilities is one of the vital unsolved challenges
in wearable communications due to the need for heterogeneous, de-
centralized, low-cost, and low-power architectures. Despite advances in
semiconductor technology and energy-efficient system design, overall
energy consumption by communications systems is still proliferating.
As users’ expectations for the networking devices’ features and battery
life continue to grow, it is imperative to optimize performance and
power consumption further. Therefore, the collection, transmission,
computation, and storage of data must be addressed consistently in
terms of power and/or time.
In dynamic Large Scale Environments (LSEs), where wearables
move around while exchanging data, issues related to scalability and
interoperability emerge to be carefully addressed. These LSEs rely
on Edge/Fog computing architectures to implement the intelligence
needed by the proximate devices and improve the quality of service
they offer. Edge/Fog architectures require adequate models with a
high degree of device autonomy and management. Since such sys-
tems typically span over a wide area and include a large number
of interacting devices, the aspects of service and object discovery,

```
and reputation assessment require intelligent management. To address
these challenges, the development of novel Edge/Fog architectures for
D2D to improve wearables’ energy efficiency and support massive,
heterogeneous, and multi-connectivity devices is required.
```
```
4.5.1. In-band/out-bandD2Dcommunication
Regarding spectrum usage, D2D communication is primarily classi-
fied into in-band and out-band. In in-band D2D communication, both
cellular and D2D communications utilize the same spectrum licensed to
the network operator, whereas out-band D2D communication operates
in an unlicensed frequency band. As pairs of devices are supposed to
be in close proximity to establish D2D communication, less transmit
power is required than while using longer-range transmissions, which
can prolong the devices’ battery life [406]. Besides, D2D communi-
cation can also result in low-transmission delay and high throughput
compared to Base Station (BS)-assisted communication. On the one
hand, the use of out-band D2D eliminates the interference between
D2D communication and network users, while at the same time, devices
have to maintain two active wireless interfaces, which leads to higher
energy consumption. On the other hand, in the case of in-band D2D,
where devices need only one active interface, the interference poses the
main issue. To handle the interference, efficient and easy-to-implement
methods are required, which pose a challenging task to the academy.
```
```
4.5.2. Packetaggregation
Wearable devices are generally physically close, thus, they perform
local end-to-end interactions with traffic that follows similar patterns.
In such a scenario, an aggregator node can collect data packets from
neighboring devices and then forward them to the final destination em-
ploying D2D technology. The advantages of adopting this forwarding
approach can be to lessen energy consumption and improve communi-
cation performance thanks to a top-notch selection of the aggregator
node and a proper setting of its transmission. As shown in [407],
using a more robust Modulation and Coding Scheme (MCS) in the
uplink can improve the energy-efficiency of communications with small
data transmissions by reducing data rate and lowering the transmission
power. In [408], the authors propose a strategy where a single device
aggregates locally generated machine-type data packets, supplements
them with its data, and then transmits them to the BS in order to
alleviate the impact of the massive number of Machine-to-Machine
(M2M) devices on a cellular system.
```
```
4.5.3. Highercellularsystemcapacity
A dense communication environment poses a challenge from the
connection establishment point of view as interference from the devices
of neighboring users can make establishing connection difficult [230].
The level flow dynamics of connectivity in wearable devices also add
further complexity to this problem. Since interference footprint from a
device can be managed by controlling the transmit power, power man-
agement [409] approaches can be utilized to minimize the interference
and potentially provide more efficient and reliable connectivity.
Generally, D2D communications allow extending the system ca-
pacity thanks to data offloading and reuse gain. Freeing up licensed
bandwidth through unlicensed D2D communications improves the scal-
ability of the system, thus allowing better management of the resources
available for the wearable environment [410]. Furthermore, due to
advances in research on methods for the interference management
between local D2D communications and the BS, resource allocation
in the cell and model selection, it is possible to implement frequency
reuse techniques that spur an increase in the network capacity. Finally,
the joint utilization of D2D communications and MEC technologies im-
proves cellular networks’ computation capacity by the tasks offloading
to a nearby D2D device and an Edge node [411].
```

```
Computer Networks 193 (2021) 108074
```
_4.5.4. Groupcommunications_
Group communications consist of one-to-many transmissions suit-
able for scenarios in which the same data must be sent to multiple de-
vices. In wearable technology, performing group communications (also
known as multicast) could help tackle energy savings, scalability, and
network traffic reduction. Furthermore, to improve the QoS offered to
all gadgets, multicast D2D communications can be established towards
devices experiencing adverse channel conditions [412]. In this case, the
forwarding mechanism requires that a device, chosen as a relay node,
after receiving the data directly from the BS, forwards it to a cluster
of devices set up using a proper approach. Researchers have proposed
many cluster-based multicast transmission methods for D2D communi-
cations [413]. Moreover, in the dynamic multi-hop multicast schemes,
the optimal number of relays must be appropriately selected by taking
into account a trade-off between multicast gain and multi-channel
diversity.

_4.5.5. Computationaloffloading_
In scenarios with low connectivity opportunities, mobile devices
may use local resources on the other devices in close proximity to
compute a common task when offloading to remote clouds fails [358].
Using D2D communication, users can improve mobile cloud comput-
ing performance in terms of computational acceleration. A significant
problem in studying D2D connectivity as an alternative to Mobile Cloud
Computing (MCC) is how users can discover and use other mobile
devices’ computing resources. Since D2D connection is usually intermit-
tent due to user mobility, access schemes need to be carefully designed.
The users can make the most of nearby mobile devices’ computing
resources without spending too much power on device discovery.

_4.6. Useradoptionaspects_

The issue of user involvement is especially acute in two areas: med-
ical and industrial. In all other situations, the use of wearable devices is
a person’s choice. It is often a matter of necessity in the case of medicine
and industry. There is a severe risk that pervasive devices, due to
their complexity and excessive ‘‘intrusiveness’’, ingenerate unnecessary
discomfort feelings and psychological stress in users. Some patients
humble themselves in the case of medical examinations since they see
a direct connection between the need for monitoring and recovery (or
maintaining their condition). Moreover, workers usually do not fully
understand the purpose of monitoring in the case of industries [414],
and attempts to implement wearable devices in industries often meet
with strong resistance from the intended users.
Nonetheless, the information ownership issue generates user distrust
of wearable technologies. The privacy reasons suggest an individual to
keep personal data as much as possible under control and to share them
only with ‘‘trusted’’ devices. The lack of attention to privacy control
would imply, for the user, a constant intolerable fear that his sphere is
violated and could ultimately lead to a state of depression. In the case of
industries, workers are often afraid that the information collected from
wearable devices could be used against them as grounds for dismissal
or transferred to third parties [415].
Another point directly related to the degree of user involvement is
their technical skills. Young people are quick to learn new technologies,
while older people, who most often need medical attention, are usually
not so good. As a result, they may prefer more traditional technologies
and resist new ones, such as wearable devices.
An essential step in overcoming the resistance of users of new tech-
nologies is creating detailed and, at the same time, simple instructions
that would explain how the device works, what data it collects, and
how this data is protected.
Finally, users want to take care of themselves. Sometimes, this
means quickly adding sensing, measurement, computation, and com-
munication devices to the platforms already in use. It should be done

```
dynamically and in a ‘‘plug-and-play’’ manner to hide differences in IoT
technology, configuration, and data format.
Another issue related to human involvement is the biological safety
under radio-frequency radiation. Health concerns attract exploding
interests from the research community due to extreme proximity and
direct physical contact with the human skin. Moreover, wearable de-
vices are recognized to cause a higher level of Specific Absorption Rate
(SAR) [416]. The SAR value is determined when the device is operating
at maximum power. The human body absorbs electromagnetic radi-
ation, which causes thermal or non-thermal radiation in the affected
tissues. In this regard, it is vital to direct the research towards regula-
tion aspects based on new device types, materials, operated frequencies,
and transmit power [214]. For instance, in [417], the exposure amounts
in different spectrum bands are investigated. Furthermore, industry
bodies should be introduced with the latest regulations to address users’
concerns better and promote this new technology.
```
```
4.7. Hardwareconstraints
```
```
Several advanced functionalities are being added to wearable de-
vices to enable new services and target new use cases. However, they
are still to be executed on tiny and resource-constrained devices. As
a result, more features may result in increased energy consumption,
which often compromises the quality of the final wearable applica-
tions. Hence, energy consumption is considered as one of the most
critical challenges in wearable computing [2]. The power alimentation
techniques of wearable devices improve with the evolution and the
increase of the user demands. For instance, the difficulty in plugging
wearable devices into power sources due to their unavailability led
to wireless charging techniques. The first commercial devices with
integrated wireless charging were cell phones. However, device manu-
facturers continued deploying these techniques in other devices, such as
laptop computers, electric vehicles, and wearables. Although it acts as
an alternate solution to regular wired charging and helps remove the
charging port from the physical design, the disadvantage of wireless
charging is that it needs long charging times [418].
When selecting a wearable device, users consider the energy con-
sumption metric as one of the top selection criteria. This fact motivated
the device manufacturers and the research community to explore tech-
niques of extending the battery life of wearable devices, i.e., increasing
energy efficiency. The research community identified three main ways
for achieving energy efficiency, namely minimizing power consump-
tion, advancing the battery techniques, and energy harvesting. First,
the energy consumption of a sensing process in several sensor-based
applications may be comparable to, or even greater than, the energy
consumption of the radio communication task [419]. Therefore, se-
lecting low-power sensors and using compressed sensing techniques
can help minimize the sensing energy consumption, thus, extending
the wearable devices’ battery lifetime. Second, the choice of com-
pact and long-lasting batteries is a significant design factor in wear-
ables. Li-ion batteries are becoming the most common type in many
wearable devices, thanks to their flexible and efficient energy-storage
features [420].
While the aforementioned energy efficiency measures can extend
wearable devices’ battery life, they cannot eliminate the need to
recharge and replace the batteries. Consequently, new energy harvest-
ing techniques have been explored to enable the use of self-powered
wearable devices. Achieving autonomy by harvesting energy from the
environment is especially attractive for wearable systems [421]. The
environment’s collected energy can be in the form of motion, temper-
ature gradients, light, electromagnetic radiation, etc. These methods
include microkinetic energy harvesting systems that use frequencies
generated by a human movement to harvest energy [422], powering
wearable devices by harvesting solar energy [423], self-powered smart
tissue [424], and wireless power transmission for implants [425,426].
```

```
Computer Networks 193 (2021) 108074
```
However, the development of energy harvesting systems for wear-
able devices has several problems compared to other traditional de-
vices. These problems are mainly related to wearable devices’ internal
limitations regarding physical size, weight, and body movement. As
a rule, modern energy harvesting efficiency is not high enough to
autonomously power wearable devices. Also, the availability of envi-
ronmental energy is not always guaranteed. Finally, energy harvest-
ing requires integrating several additional hardware components on
board, such as environmental energy collectors, additional batteries
to store the collected energy, etc., which becomes a challenge when
considering a small form factor. Therefore, a significant amount of
research is required in this direction so that future wearable devices
can continuously generate energy from external sources [427].

Self-powered devices are not considered the last step towards
energy-efficient operations of wearables. The circuit technology ad-
vances aim to reduce the device power consumption up to keeping
them perpetually alive. As a result, a future breakthrough for achieving
always-on things in IoT is the concept of zero-energy devices [428].
This concept is based on zero-power sensing, where all the energy
needed for the measurement data is generated by the specific phys-
ical phenomenon being measured. Therefore, no other power supply
sources need to be present in the system. The generation of the energy
from the measured phenomenon is performed using two fundamental
enablers for zero-energy devices, namely Wireless Energy Transfer
(WET) and backscatter technologies.

_4.8. Interoperabilityaspects_

While academia, industry, and standardization bodies have shown
a substantial interest in developing solutions for the IoWT ecosystem,
there are still multiple aspects requiring additional attention, including
scalability, mobility, dynamicity, heterogeneity and interoperability,
adaptability, security, standards, etc. Among these challenges, _interop-
erability_ is one of the main issues since various components, objects,
communication technologies, applications, services, etc., need to seam-
lessly cooperate and interact with each other to realize the full potential
of the automated IoWT systems [429].

Despite the impressive potentialities of such systems, the full inte-
gration between IoWT and, e.g., eHealth systems are still far from an
actual implementation. Two main factors hinder such an integration.
The first issue is focused on the interoperability between eHealth
devices and wearables. Reference architectures and protocols devised
so far for eHealth and IoWT exhibit many differences. The second one
involves managing the potentially numerous and heterogeneous node
candidates integrated into the eHealth platforms.

Moreover, _personalization_ and _interoperability_ represent two corner-
stones of eHealth systems [176]. Each patient has their peculiarities:
one can be computer literate or not, mostly healthy or seriously ill,
more prone or reluctant to accept a given treatment (e.g., due to cul-
tural biases). On the other hand, pathologies have their characteristics,
and each one requires specific treatment and monitoring. As a result,
it is impossible to devise a single one-fits-all eHealth platform; instead,
patients need to rely on various personalized solutions. The only way
to economically achieve the required high degree of personalization
is to construct eHealth systems based on basic devices with a high
technological interoperability level.

Most of the attempts to integrate IoWT and eHealth systems carried
out so far aim at achieving full interoperability between eHealth de-
vices and wearables. The main idea is to transport part of the ISO/IEEE
11073-20601 over protocols typically used in the IoT [434] or widely

```
diffused in Consumer Electronic devices [435]. The work [434] also
proposes to transport ISO/IEEE 11073-2060 messages over the
CoAP [445] with Representational state transfer (REST) API, which has
been designed by the Internet Engineering Task Force (IETF) Constrained
RESTful Environments (CORE) Working Group [446] also approach to
constrained nodes.
CoAP is considered the reference Web transfer protocol to en-
able the inclusion of the simplest object in the Web. The transport
of ISO/IEEE 11073-20601 over CoAP is not straightforward. While
communications in CoAP are initiated from a client towards a server,
both a manager or a client can initiate a communication in ISO/IEEE
11073-20601. This discrepancy requires the deployment of a CoAP
client and a CoAP server on the manager and agents, thus increasing
the computational load of devices.
Similarly to [435], the work [447] proposes to transport ISO/IEEE
11073-20601 messages over the UPnP protocol, a technology intro-
duced by the Digital Living Network Alliance (DLNA). This open net-
work architecture enables discovery and control of networked devices
and services and is widely deployed in modern Consumer Electronic
(CE) devices, such as media servers and smart TV. Besides basic com-
munication features, UPnP also provides management features as a de-
vice discovery mechanism that allows applications to opportunistically
use the nodes near a patient with no prior knowledge.
In [434,435], the Application Hosting Device (AHD) was chosen as
the conjunction point between the Continua architecture and IoT. In
other words, this is the device where ISO/IEEE 11073-20601 is mapped
onto CoAP/UPnP AHD plays this role because it is the device closest to
the patient and powerful enough to run multiple protocols and perform
complex operations.
Other proposals in the literature retrofit biometric sensors with
CoAP, but are either non-compliant with the continua guidelines or
with the ISO/IEEE 11073 standard set [448]. It cannot be considered a
real integration with the legacy eHealth system, which will continue
to represent and exchange information according to their standards.
Therefore, most of the benefits coming from the integration are lost.
Abstracting from the integration of the IoWT and eHealth systems,
the work [279] presents the open challenges of IoT interoperability
needed to be solved. One of the open challenges is ensuring the in-
teroperability of IoWT applications and solutions from all perspectives
such as devices, networks, and others (for more details, see Section 3).
In contrast, the current solutions face interoperability from a specific
perspective only. This finding highlights the direction for future IoWT
adoption. Another area of the research work identified in [279] is the
implementation of scalable interoperability solutions able to ensure
reliable D2D connectivity [449] between devices with different com-
putational capabilities (e.g., high-end and low-end devices). Moreover,
with the enormous current interest in digitalization, the transition
toward distributed cloud computing is an inherent part of future 5G and
beyond platforms. It is crucial to develop interoperability solutions for
different platforms and applications with a high level of flexibility in
this context. Finally, it is vital to address interoperability between more
than a couple of platforms. Solutions must be realistic and scalable
across multiple platforms regardless of the area and domain, scenarios,
and even utilized technologies.
To sum it up, seamless and ubiquitous communications are expected
to accelerate technological innovation, increase productivity and relia-
bility, and open up new opportunities for IoWT technologies. Therefore,
end-to-end solutions for wearable things that offer seamless integration
into existing systems and processes are of great concern. Moreover,
it is essential to note that weight, size, power, durability, reliability,
and ease of use are key considerations in finding solutions for the
end-users [450].
```

```
Computer Networks 193 (2021) 108074
```
```
Table 6
Summary of the main challenges related to modern wearable technology (sorted alphabetically).
Challenge Groups Refs. Observed existing approach
Appropriate service/DT placement and
migration
```
```
A, DP [430] Utilization of an algorithm for replica placement
[366] An algorithm for the optimal migration strategy of services based on dynamic programming
[367] A model for resource management based on the regularization technique
[368] A framework to design optimal service migration policies based on Markov decision process
Data collection issues DP, SW [336,337] Development and application of a unified, trusted crowdsourcing platforms
Datasets’ imbalance DP [431] The application of data augmentation methods for imbalanced datasets and weighting architecture
Energy overheads related to sensing DP, HW, SW [419] Following of the sensing energy consumption minimization strategy
A feeling of constant surveillance UR [414,432] A detailed explanation of the purpose of the monitoring and what is going to be done with the
collected data
[433] Providing the user with privacy and security of collected data
Inefficient computing resources
detection
```
```
A, N [358] Carefully developed access shames allowing the users to utilize nearby mobile devices’ computing
resources as much as possible while not wasting too much energy on other devices’ discovery
Inefficient data analytics DP, SW [338,339] Application of techniques from the field of statistics and ML
Inefficient switching among resources
in hybrid/heterogeneous networks
```
```
A, N, HW [359–361] Selection and utilization of improved task offloading schemes
```
```
Insufficient computing capabilities A, N, HW [358] The use of D2D communication to improve mobile cloud computing’s performance
Lack of appropriate data labeling DP [340,341] Application of semi-supervised methods
Lack of direct interoperability between
eHealth devices
```
```
A, DP [434] A system architecture based on IEEE 11073, Constraint Application Protocol (CoAP), and Universal
Plug and Play (UPnP)
[435] A reference implementation based on Transmission Control Protocol/Internet Protocol (TCP/IP),
CoAP
Lack of modern energy harvesting
opportunities
```
```
HW [422] The use of micro-kinetic energy harvesting systems
[423] Powering wearables with solar energy harvesting
[424]] The application of self-powering smart fabric
[425,426] The integration of wireless power transfer option for implantables
[427] Continuous power generation from ambient sources
Lack of network resources A, N [410] The application of D2D to extend the system capacity thanks to data offloading and reuse gain
[411] The use of D2D-MEC system to improve the computation capacity of the whole system
Problems related to broadcast
communications
```
```
A, N [412] Group communications (multicast transmission)
```
```
Limited amount of the available data DP [195] Extension of the available data by applying the data augmentation techniques
Low data quality DP [160] The application of post-processing techniques to improve the quality
Low data resolution DP [335] The utilization of active and passive data collection approaches to increase the resolution
Low QoS indicator A, N [413] Cluster-based multicast transmission methods for D2D communications
Low technical skills UR [415] A detailed guidance and training including seminars and interactive lessons for every age group
[436,437] Friendly and responsive customer support
Non-optimized security and privacy
enablers
```
```
HW, DP, SW [438] Content agnostic privacy and encryption protocol eliminating the need for asymmetric encryption
```
```
[393,439] Integration of lightweight cryptography solutions including more appropriate elliptic curve types
or algorithm implementations
[440] More efficient utilization of manufacturer-provide System on Chip (SOC)s accelerated for
cryptographic primitives execution
[441] Finding trade-offs between the primitive and required level of the provided security
Problems of classification, anomaly
detection, forecasting problems
```
```
DP, SW [442–444] The application of ML approaches
```
```
A – Architecture; N – Networking; DP – Data Processing; HW – Hardware specific; SW – Software specific; UR – User-related.
```
_4.9. Management/scalabilityaspects_

The IoWT paradigm is rooted in the simple consideration that the
space around us is saturated by a multitude of devices connected to
the Internet and unequivocally addressable [451]. The devices usually
have limited capabilities when considered singularly, but they become
capable of very complex operations when a few cooperate, to say it in
a motto: _Theirnumberistheirstrength_.
However, the efficient management of the considerable IoWT de-
vices’ number is not straightforward to achieve, and maybe the most
prominent factor which hinders the full accomplishment of the IoWT
paradigm [452]. Wearables are usually utilized by single users/com-
panies with high mobility patterns. Therefore, it becomes close to
impossible to define the number of available nodes in a given area, their
capabilities, and the way of their integration to solve a given problem.

```
The scientific community is only scarcely working on devising
proper ways to manage billions of devices, which will populate the
forthcoming IoWT [452]. The issue is still open, and very few proposals
are focused explicitly on integrating the IoWT in today’s networks.
```
```
4.10. Sectionsummary
```
```
This section outlined the main challenges present in modern and
future wearable devices and underlying technologies. The summary of
the most significant ones is presented in Table 6.
These challenges are still unresolved because they are extremely
complex and limited by various factors locked in small form-factor
devices. Current research efforts are fragmentary and very narrow in
scope. They focus either on the machine-centric perspective or on the
human-centric perspective, which results in a lack of synergy. Solving
```

```
Computer Networks 193 (2021) 108074
```
the challenges described above requires a unique, multidisciplinary,
and inter-sectoral approach and a concerted effort of the best experts
from all over the world to make progress beyond the state-of-the-art.

**5. Review summary**

The evolution of modern electronics towards miniaturization paves
the way for a relatively young segment of IoT devices – wearables,
the ones we carry and wear on us daily. Indeed, the main building
block for mass adoption and broad integration of modern wearables
is technology, including computation, communication, battery, chip
size aspects, among many others. The history of wearables, provided
in detail in this paper, is enormous and dates hundreds of years ago,
leading to the devices currently surrounding people and soon joining
our ecosystems.
As for modern devices, evolving from the first healthcare devices
and conventional activity trackers, different wearables are presently
found on various parts of our body, mainly depending on the appli-
cation scenario and data collection/output needs. Wearables of today
preliminary communicate via short-range wireless technology, with
few exceptions based on infrastructure connectivity. This tendency is
mainly due to present battery limitations and the overheads brought
by higher power consumption while using longer-range communication
technology. Nonetheless, most wearables are still utilized for data col-
lection purposes requiring sophisticated techniques to achieve higher
efficiency of the entire data processing life cycle. However, the tight
coupling of various systems provided by different vendors is still one
of the most significant challenges of wearables due to the lack of good-
practices on interoperability and the appropriate standardization in the
young IoWT niche.
To summarize, wearable technology is an essential building block in
the future ICT systems. It is still in its infancy, and several critical chal-
lenges from data acquiring and processing, communications, security,
privacy aspects, hardware limitations, and user adoption are still to be
addressed. This paper highlights those and provides the readers with
an excessive summary of potential solutions to overcome the present
literature.

**CRediT authorship contribution statement**

**Aleksandr Ometov:** Project administration, Data curation, Visual-
ization, Writing – original draft. **Viktoriia Shubina:** Writing – original
draft, Writing – review & editing. **Lucie Klus:** Visualization, Writing –
review & editing. **Justyna Skibińska:** Writing – review & editing.
**Salwa Saafi:** Writing – review & editing. **Pavel Pascacio:** Writing – re-
view & editing. **Laura Flueratoru:** Writing – review & editing. **Darwin
Quezada Gaibor:** Writing – review & editing. **Nadezhda Chukhno:**
Writing – review & editing. **Olga Chukhno:** Writing – review &
editing. **Asad Ali:** Writing – review & editing. **Asma Channa:** Writing –
review & editing. **Ekaterina Svertoka:** Writing – review & editing.
**Waleed Bin Qaim:** Writing – review & editing. **Raúl Casanova-
Marqués:** Writing – review & editing. **Sylvia Holcer:** Writing – re-
view & editing. **Joaquín Torres-Sospedra:** Writing – review & editing.
**Sven Casteleyn:** Writing – review & editing. **Giuseppe Ruggeri:**
Writing – review & editing. **Giuseppe Araniti:** Writing – review &
editing. **Radim Burget:** Writing – review & editing. **Jiri Hosek:** Writ-
ing – review & editing. **Elena Simona Lohan:** Project administration,
Writing – review & editing.

**Declaration of competing interest**

The authors declare that they have no known competing finan-
cial interests or personal relationships that could have appeared to
influence the work reported in this paper.

```
Acknowledgments
```
```
This work was supported by European Union’s Horizon 2020 Re-
search and Innovation programme under the Marie Skłodowska Curie
grant agreement No. 813278 (A-WEAR: A network for dynamic WEar-
able Applications with pRivacy constraints), http://www.a-wear.eu/
```
```
List of Acronyms
```
```
3G The Third Generation Cellular Network Technology
3GPP The 3rd Generation Partnership Project
5G The Fifth Generation Cellular Network Technology
A-WEAR A Network for Dynamic Wearable Applications with Privacy
Constraints
AAFT Adjusted Fourier Transform
ACES Asynchronous Coded Electronic Skin
AHD Application Hosting Device
AHL Asymmetric Hearing Loss
AOA Angle of Arrival
AI Artificial Intelligence
ALS Amyotrophic Lateral Sclerosis
API Application Programming Interface
AR Augmented Reality
ATM Automated Teller Machine
BAN Body Area Network
BLE Bluetooth Low Energy
BS Base Station
BLSTM Bidirectional Long Short-Term Memory
CAGR Compound Annual Growth Rate
CE Consumer Electronic
CES Consumer Electronics Show
CSI Channel State Information
CHF congestive heart failure
CoAP Constraint Application Protocol
CORE Constrained RESTful Environments
CNN Convolutional Neural Network
CH Cluster Head
D2D Device-to-Device
DLNA Digital Living Network Alliance
DHKE Diffie-Hellman Key Exchange
DT Digital Twin
DTW Dynamic Time Warping
ECG Electrocardiogram
EEG Electroencephalogram
FPV First-person view
eMTC enhanced Machine Type Communication
GNSS Global Navigation Satellite System
GLONASS Global Navigation Satellite System
GPRS General Packet Radio Services
GDPR General Data Protection Regulation
GPS Global Positioning System
GRU Gated Recurrent Units
H2H Human-to-Human interaction
HAR Human Activity Recognition
HMD Head-Mounted Display
HRD Health Recording Devices
HW Hardware
HC-RAN Heterogeneous Cloud Radio Access Network
HCI Human-Computer Interaction
IAAFT Iterated Adjusted Fourier Transform
ICD Industrial Clothing Division
```

```
Computer Networks 193 (2021) 108074
```
**ICT** Information and Communications Technology
**IDDS** Insertable Drug Deliverables Systems
**IEEE** Institute of Electrical and Electronics Engineers
**IETF** Internet Engineering Task Force
**IF** Interface
**IIoT** Industrial Internet of Things
**ILS** Indoor Location Systems
**IoT** Internet of Things
**IoWT** Internet of Wearable Things
**ITB** Inside-the-body
**IPS** Indoor Positioning System
**IEC** International Electrotechnical Commission
**IP** Ingress Protection Code
**IR** Identifiable Infrared
**ISM** Industrial, Scientific, and Medical
**ISO** International Organization for Standardization
**KARMA** Knowledge-based Augmented Reality for Maintenance
Assistance
**LAN** Local Area Network
**LBS** Location-Based Service
**LSI** Large-Scale Integration
**LED** Light-emitting diode
**LPWA** Low-Power Wide Area
**LPWAN** Low-Power Wide Area Network (protocols)
**LSE** Large Scale Environment
**LSTM** Long Short-Term Memory
**LTE** Long Term Evolution
**LoRa** Long Range LPWAN protocol
**LOS** Line-of-Sight
**MAC** Medium Access Control
**M2M** Machine-to-Machine
**MCC** Mobile Cloud Computing
**MCS** Modulation and Coding Scheme
**MEC** Multi-Access Edge Computing (formely Mobile Edge
Computing)
**mMTC** Massive Machine Type Communications
**mmWave** Millimeter Wave
**MR** Mixed Reality
**MRI** Magnetic Resonance Imaging
**MS** Multiple Sclerosis
**MTC** Machine Type Communications
**MLP** Multilayer Perceptron
**ML** Machine Learning
**MIMO** Multiple Input Multiple Output
**MWC** Mobile WOrld Congress
**NB-IoT** Narrowband Internet of Things
**NFC** Near Field Communication
**NLOS** Non-Line-of-Sight
**OGC** Open Geospatial Consortium
**OS** Operating System
**P2P** Peer-to-Peer
**PAN** Personal Area Network
**POA** Phase of Arrival
**PoW** Proof of Work
**PDA** personal digital assistant
**QoS** Quality of Service
**RAM** Random-access memory
**RAN** Radio Access Network
**RAT** Radio Access Technology
**REST** Representational state transfer

```
RF Radio Frequency
RC Remote control
RFID Radio Frequency Identification
RNSS Regional Navigation Satellite Systems
RSS Received Signal Strength
SAR Specific Absorption Rate
SDN Software-Defined Networks
SIM subscriber identification module
SIoT Social Internet of Things
SOC System on Chip
SSD single-sided deafness
SW Software
SW Software
TCP/IP Transmission Control Protocol/Internet Protocol
THz Terahertz
TOA Time-of-Arrival
UPnP Universal Plug and Play
UWB Ultra-Wide Band
VLC Visible Light Communications
VR Virtual reality
WAN Wide Area Network
WBAN Wireless Body Area Network
WPAN Wireless Personal Area Network
WSN Wireless Sensor Network
WET Wireless Energy Transfer
Wi-Fi Wireless Fidelity
WiGig Wireless Gigabit Alliance (WiFi at 60 GHz)
WLAN Wireless Local Area Network
XR eXtended reality
```
```
Appendix. Description of the wearable devices’ dataset
```
```
During the preparation of this survey, our team has analyzed the
market and exiting research projects, which resulted in the dataset
allowing for easy analysis of the available wearable devices. The most
recent version of the dataset is available via Zenodo repository https:
//zenodo.org/record/4575153. As of the paper submission date, it
provides the data about 224 wearable devices.
In particular, it consists of the following fields (some fields could be
empty due to the unavailability of the module):
```
- **Device** – name of the wearable on the market or project title;
- **Location type** – data on the wearablity, based on the proposed
    classification;
- **Application type** based on the proposed classification;
- **Device type** based on the proposed classification;
- **Hi/low end** – type of the device according to its’ functionality;
- **Prototype** or availability on the market;
- **Energy-related information** – information either on power sup-
    ply or on the battery type;
- **CPU** – information about the processor;
- **GPU** – information about the graphical card;
- **Camera** – information about the camera(s);
- **Cellular** – information about the cellular module and technology;
- **WiFi** – information about the WiFi module and technology;
- **Bluetooth** – information about Bluetooth module and, optionally,
    version;
- **RFID** – information about RFID module;
- **Other connectivity** – the list of other connectivity options
    present on the device;
- **GNSS** – information about conventional positioning systems;
- **RAM** – information about integrated RAM;


```
Computer Networks 193 (2021) 108074
```
- **Storage** – information about available internal storage or slots
    available for external memory stick;
- **Display** – information about the graphical output interface;
- **Audio output** – information about audio output devices;
- **Mic** – presence of audio input interface;
- **Release** – first release date or year;
- **Price $** – market price as of 2020;
- **Luxury** – information if the device could be considered as a
    luxury accessories;
- **Activity tracking** – presence of the activity tracking feature with
    details;
- **Sensors** – list of the sensors and actuators integrated in the
    device;
- **Description** (optional) – short description of the device;
- **Other comments** – additional notes on the device;
- **Link** – example link with the device information.

```
An example of one entry could be found in the following listing:
```
```
[ 1
{ 2
" Device " : " Focals by North " , 3
" Location type " : " Head_mounted " , 4
" Application type " : " Eyewear " , 5
" Device type " : "AR" , 6
" Hi or low end" : " high " , 7
" Prototype " : " yes " , 8
" Energy−related information " : "700 mAh/18 hours " , 9
"CPU" : "Qualcomm APQ8009w" , 10
"GPU" : "n/a" , 11
"Camera" : " yes " , 12
" Cellular " : "no" , 13
" WiFi " : "no" , 14
" Bluetooth " : " yes " , 15
"RFID" : "no" , 16
" Other connectivity " : "no" , 17
"GNSS" : "no" , 18
"RAM" : "n/a" , 19
" Storage " : "n/a" , 20
" Display " : " yes " , 21
" Audio output " : " yes " , 22
"Mic" : " yes " , 23
" Release " : "n/a" , 24
" Price $" : "n/a" , 25
" Lyxury " : " yes " , 26
" Acitivity tracking " : " yes " , 27
" Sensors " : "9−axis IMU, Ambient Light Sensor , 28
Proximity sensor " , 29
" Description " : " Smart AR glasses. Could be 30
used as handsfree and with assistants. " , 31
" Other comments" : " IP55" , 32
" Link " : " https : //www. bynorth .com/tech " 33
} , 34
<... > 35
] 36
```
**References**

```
[1] Cisco Visual Networking Index, Global Mobile Data Traffic Forecast Update,
2017–2022 White Paper, 2019, [Online] https://www.cisco.com/c/en/us/
solutions/collateral/service-provider/visual-networking-index-vni/white-paper-
c11-738429.html (Accessed March 3, 2021).
[2] W.B. Qaim, A. Ometov, A. Molinaro, I. Lener, C. Campolo, E.S. Lohan, J. Nurmi,
Towards Energy Efficiency in the Internet of Wearable Things: A Systematic
Review, IEEE Access.
[3] T. Luczak, R. Burch, E. Lewis, H. Chander, J. Ball, State-of-the-Art Review of
Athletic Wearable Technology: What 113 Strength and Conditioning Coaches
and Athletic Trainers from the USA Said about Technology in Sports, Int. J.
Sports Sci. Coach. 15 (1) (2020) 26–40.
```
```
[4] S. Khan, S. Parkinson, L. Grant, N. Liu, S. Mcguire, Biometric Systems Utilising
Health Data from Wearable Devices: Applications and Future Challenges in
Computer Security, ACM Comput. Surv. 53 (4) (2020) 1–29.
[5] J. Zhou, Z. Cao, X. Dong, N. Xiong, A.V. Vasilakos, 4S: A Secure and Privacy-
Preserving Key Management Scheme for Cloud-Assisted Wireless Body Area
Network in m-Healthcare Social Networks, Inform. Sci. 314 (2015) 255–276.
[6] A. Ometov, Social, Private, and Trusted Wearable Technology under Cloud-
Aided Intermittent Wireless Connectivity (Ph.D. thesis), Tampere University of
Technology, 2018.
[7] S. Tweedie, The World’s First Smartphone, Simon, Was Created 15 Years Before
the iPhone, Bus. Insider (2019) [Online] https://www.businessinsider.com/
worlds-first-smartphone-simon-launched-before-iphone-2015-6?r=US&IR=T
(Accessed March 3, 2021).
[8] Business Wire Inc., The Wearable Technology Ecosystem: 2016-2030 –
Opportunities, Challenges, Strategies, Industry Verticals and Forecasts
for the $40 Billion Market – Research and Markets, 2016, [Online]
https://www.businesswire.com/news/home/20160504005813/en/Wearable-
Technology-Ecosystem-2016-2030---Opportunities-Challenges (Accessed March
3, 2021).
[9] I-SCOOP, Wearables Market Outlook 2020: Drivers and New Markets, 2016,
[Online] https://www.i-scoop.eu/wearables-market-outlook-2020-drivers-new-
markets/ (Accessed March 3, 2021).
[10] J. Hayward, Wearable Sensors 2018-2028: Technologies, Markets & Players,
IDTechEx Ltd, 2018.
[11] J. Smith, Wearables Shipments Will Double By 2021, Insider Inc, 2017,
[Online] https://www.businessinsider.com/wearables-shipments-will-double-
by-2021-2017-12?r=US&IR=T (Accessed March 3, 2021).
[12] J. Hayward, Wearable Technology Forecasts: 2020-2030, IDTechEx, 2020,
[Online] https://www.idtechex.com/en/research-report/wearable-technology-
forecasts-2020-2030/747 (Accessed March 3, 2021).
[13] M.T. Rashid, D. Wang, CovidSens: A Vision on Reliable Social Sensing for
COVID-19, Artif. Intell. Rev. (2020) 1–25.
[14] E. Hernández-Orallo, P. Manzoni, C.T. Calafate, J.-C. Cano, Evaluating How
Smartphone Contact Tracing Technology Can Reduce the Spread of Infectious
Diseases: The Case of COVID-19, 2020, IEEE Access.
[15] A.K. Tripathy, A.G. Mohapatra, S.P. Mohanty, E. Kougianos, A.M. Joshi, G. Das,
EasyBand: A Wearable for Safety-Aware Mobility during Pandemic Outbreak,
IEEE Consum. Electron. Mag..
[16] V. Shubina, A. Ometov, E.S. Lohan, Technical Perspectives of Contact-Tracing
Applications on Wearables for COVID-19 Control, in: Proc. of 12th International
Congress on Ultra Modern Telecommunications and Control Systems and
Workshops (ICUMT), IEEE, 2020, pp. 229–235.
[17] R.T. Llamas, Enterprise Wearable Market: Information By Technology (IoT,
Bluetooth, BLE), Product (Wristwear, Footwear, Eyewear), Application (Info-
tainment, IT), and Regional Outlook – Forecast Till 2026, Tech. Rep. SR1195,
Straits Research, 2019.
[18] DVV Media HR Group Ltd, The Benefits of Wearable Technology in the Work-
place, 2018, [Online] https://www.employeebenefits.co.uk/benefits-wearable-
technology-workplace/ (Accessed March 3, 2021).
[19] Guardian24 Ltd, 4 Benefits of Wearable Technology, 2017, [Online] https:
//guardian24.co.uk/4-benefits-of-wearable-technology/ (Accessed March 3,
2021).
[20] N. Costa, 6 Ways Wearable Tech Makes Everything Better (in Work and
Life), Koombea, Inc, 2018, [Online] https://www.koombea.com/blog/6-ways-
wearable-tech-makes-everything-better/ (Accessed March 3, 2021).
[21] R.T. Llamas, IDC Forecasts Steady Double-Digit Growth for Wearables As
New Capabilities and Use Cases Expand the Market Opportunities, Inter-
national Data Group (IDG), 2019, [Online] https://www.idc.com/getdoc.jsp?
containerId=prUS44930019 (Accessed March 3, 2021).
[22] Welbi, 5 Health Benefits of Wearable Tech, 2019, [Online] https://www.welbi.
co/single-post/5-health-benefits-of-wearable-tech (Accessed March 3, 2021).
[23] C. Kresser, The benefits of using wearable technology for health track-
ing, 2019, [Online] https://chriskresser.com/the-benefits-of-using-wearable-
technology-for-health-tracking/ (Accessed March 3, 2021).
[24] A. Ometov, D. Kozyrev, V. Rykov, S. Andreev, Y. Gaidamaka, Y. Koucheryavy,
Reliability-centric Analysis of Offloaded Computation in Cooperative Wearable
Applications, Wirel. Commun. Mob. Comput., 2017.
[25] M. Pedram, M. Rofouei, F. Fraternali, Z.E. Ashari, H. Ghasemzadeh,
Resource-Efficient Computing in Wearable Systems, arXiv preprint arXiv:1907.
03247.
[26] O. Galinina, H. Tabassum, K. Mikhaylov, S. Andreev, E. Hossain, Y. Kouch-
eryavy, On Feasibility of 5G-grade Dedicated RF Charging Technology for
Wireless-Powered Wearables, IEEE Wirel. Commun. 23 (2) (2016) 28–37.
[27] Y. Li, Y. Chen, C.S. Chen, Z. Wang, Y.-h. Zhu, Charging while Moving:
Deploying Wireless Chargers for Powering Wearable Devices, IEEE Trans. Veh.
Technol. 67 (12) (2018) 11575–11586.
[28] M. Cheikh, Y. Vassilieff, A. Fortes, R. Benbouhout, H. Foligné, Human body
exposure to low frequency wireless charging: Direct coupling mechanisms and
interferences with medical devices, in: Proc. of Progress in Electromagnetics
Research Symposium-Fall (PIERS-FALL), IEEE, 2017, pp. 1048–1054.
```

```
Computer Networks 193 (2021) 108074
```
[29] B. Garland, Future of Wireless Charging, TechNative, 2018, [Online] https:
//www.mymemory.co.uk/blog/future-of-wireless-charging/ (Accessed March 3,
2021).
[30] S. Seneviratne, Y. Hu, T. Nguyen, G. Lan, S. Khalifa, K. Thilakarathna, M.
Hassan, A. Seneviratne, A Survey of Wearable Devices and Challenges, IEEE
Commun. Surv. Tutor. 19 (4) (2017) 2573–2620.
[31] J.J. Ferreira, C.I. Fernandes, H.G. Rammal, P.M. Veiga, Wearable Technology
and Consumer Interaction: A Systematic Review and Research Agenda,
Comput. Hum. Behav. 118 (2021) 106710, [http://dx.doi.org/10.1016/j.](http://dx.doi.org/10.1016/j.)
chb.2021.106710, URLhttps://www.sciencedirect.com/science/article/pii/
S0747563221000327.
[32] Y. Xue, A Review on Intelligent Wearables: Uses and Risks, Hum. Behav.
Emerg. Technol. 1 (4) (2019) 287–294, [http://dx.doi.org/10.1002/hbe2.173,](http://dx.doi.org/10.1002/hbe2.173,)
arXiv:https://onlinelibrary.wiley.com/doi/pdf/10.1002/hbe2.173 URL https://
onlinelibrary.wiley.com/doi/abs/10.1002/hbe2.173.
[33] N. Niknejad, W.B. Ismail, A. Mardani, H. Liao, I. Ghani, A Comprehensive
Overview of Smart Wearables: The State of the Art Literature, Recent Advances,
and Future Challenges, Eng. Appl. Artif. Intell. 90 (2020) 103529, [http://dx.](http://dx.)
doi.org/10.1016/j.engappai.2020.103529, URL https://www.sciencedirect.com/
science/article/pii/S0952197620300348.
[34] W.A.D.M. Jayathilaka, K. Qi, Y. Qin, A. Chinnappan, W. Serrano-Garcí a, C.
Baskar, H. Wang, J. He, S. Cui, S.W. Thomas, S. Ramakrishna, Significance of
Nanomaterials in Wearables: A Review on Wearable Actuators and Sensors, Adv.
Mater. 31 (7) (2019) 1805921, [http://dx.doi.org/10.1002/adma.201805921,](http://dx.doi.org/10.1002/adma.201805921,)
arXiv:https://onlinelibrary.wiley.com/doi/pdf/10.1002/adma.201805921 URL
https://onlinelibrary.wiley.com/doi/abs/10.1002/adma.201805921.
[35] C. McCallum, J. Rooksby, C.M. Gray, Evaluating the Impact of Physical Activity
Apps and Wearables: Interdisciplinary Review, JMIR Mhealth Uhealth 6 (3)
(2018) e58, [http://dx.doi.org/10.2196/mhealth.9054,](http://dx.doi.org/10.2196/mhealth.9054,) URL [http://mhealth.jmir.](http://mhealth.jmir.)
org/2018/3/e58/.
[36] P.J. Soh, G.A. Vandenbosch, M. Mercuri, D.M.-P. Schreurs, Wearable Wireless
Health Monitoring: Current Developments, IEEE Microwave Mag. 16 (4) (2015)
55–70.
[37] A. Mosenia, S. Sur-Kolay, A. Raghunathan, N.K. Jha, Wearable Medical Sensor-
based System Design: A Survey, IEEE Trans. Multi-Scale Comput. Syst. 3 (2)
(2017) 124–138.
[38] J.M. Peake, G. Kerr, J.P. Sullivan, A Critical Review of Consumer Wearables,
Mobile Applications, and Equipment for Providing Biofeedback, Monitor-
ing Stress, and Sleep in Physically Active Populations, Front. Physiol. 9
(2018) 743, [http://dx.doi.org/10.3389/fphys.2018.00743,](http://dx.doi.org/10.3389/fphys.2018.00743,) URL https://www.
frontiersin.org/article/10.3389/fphys.2018.00743.
[39] P. Kumari, L. Mathew, P. Syal, Increasing Trend of Wearables and Multimodal
Interface for Human Activity Monitoring: A Review, Biosens. Bioelectron. 90
(2017) 298–307.
[40] The College of Optometrists, The Invention of Spectacles: How and
Where Glasses May Have Begun, 2019, [Online] https://www.college-
optometrists.org/the-college/museum/online-exhibitions/virtual-spectacles-
gallery/the-invention-of-spectacles.html (Accessed March 3, 2021).
[41] T. Cassidy, A Short History of Spectacles,
[42] G. Oestmann, The Origins and Diffusion of Watches in the Renaissance:
Germany, Comune di Cremona, 2016, pp. 141–143.
[43] Oldest.org, 10 Oldest Watches in the World, 2019, [Online] [http://www.oldest.](http://www.oldest.)
org/technology/watches/(Accessed March 3, 2021).
[44] D. Boettcher, The Invention of the Wristwatch, 2019, [Online] https://www.
vintagewatchstraps.com/wristwatchinvention.php (Accessed March 3, 2021).
[45] U. Friedman, A Brief History of the Wristwatch: The Military Ori-
gins of Wearable Tech, a Century Before the Apple Watch, 2015,
[Online] https://www.theatlantic.com/international/archive/2015/05/history-
wristwatch-apple-watch/391424/ (Accessed March 3, 2021).
[46] E. Zolfagharifard, Is This the First Wearable Computer? 300-year-Old Chinese
Abacus Ring was Used During the Qing Dynasty to Help Traders, Daily Mail
(2014) [Online] https://www.dailymail.co.uk/sciencetech/article-2584437/Is-
wearable-computer-300-year-old-Chinese-abacus-ring-used-Qing-Dynasty-
help-traders.html(Accessed March 3, 2021).
[47] T. Berman, The Smart Ring: From the 17th Century Wearable Abacus
to Today, 2017, [Online] https://interestingengineering.com/smart-ring-17th-
century-wearable-abacus-today (Accessed March 3, 2021).
[48] The Public Domain Review, Dr Julius Neubronner’s Miniature Pigeon
Camera, 2019, [Online] https://publicdomainreview.org/collections/dr-julius-
neubronners-miniature-pigeon-camera/ (Accessed March 3, 2021).
[49] A. DenHoed, The Turn-of-the-Century Pigeons That Photographed Earth from
Above, 2018, [Online] https://publicdomainreview.org/collections/dr-julius-
neubronners-miniature-pigeon-camera/(Accessed March 3, 2021),
[50] The National Archives, Fighting talk: First World War Telecommuni-
cations, 2019, [Online] [http://www.nationalarchives.gov.uk/first-world-war/](http://www.nationalarchives.gov.uk/first-world-war/)
telecommunications-in-war/ (Accessed March 3, 2021).
[51] D. Hinhs, Walkie Talkie, 2019, [Online] [http://www.dlhings.ca/walkietalkie.](http://www.dlhings.ca/walkietalkie.)
html (Accessed March 3, 2021).

```
[52] G. Myre, From Wristwatches To Radio, How World War I Ushered in
the Modern World, NPR, 2017, [Online] https://www.npr.org/sections/
parallels/2017/04/02/521792062/from-wristwatches-to-radio-how-world-war-
i-ushered-in-the-modern-world?t=1568188507348 (Accessed March 3, 2021).
[53] J. Stamp, A Partial History of Headphones, 2013, [Online] https:
//web.archive.org/web/20130409012634/http://blogs.smithsonianmag.com/
design/2013/03/a-partial-history-of-headphones/ (Accessed March 3, 2021).
[54] B. Ticknor, Virtual Reality and the Criminal Justice System: Exploring the
Possibilities for Correctional Rehabilitation, Lexington Books, 2018.
[55] M.L. Heilig, Sensorama simulator, 1962.
[56] B. Rhodes, A Brief History of Wearable Computing, MIT, 2019, [Online]
https://www.media.mit.edu/wearables/lizzy/timeline.html (Accessed March 3,
2021).
[57] E.O. Thorp, Beat the Dealer: A Winning Strategy for the Game of Twenty One,
Vol. 310, Vintage, 1966.
[58] E.O. Thorp, The Invention of the First Wearable Computer, in: Digest of Papers.
Second International Symposium on Wearable Computers (Cat. No. 98EX215),
IEEE, 1998, pp. 4–8.
[59] E. Kurland, History of VR, in: Virtual Reality Filmmaking, Routledge, 2017, pp.
7–17.
[60] E. Ackerman, The Man Who Invented VR Goggles 50 years Too Soon, IEEE
Spectr. (2016).
[61] T. Emerson, Mastering the Art of VR: On Becoming the HIT Lab Cybrarian,
Electron. Libr. 11 (6) (1993) 385–391.
[62] S.D. Guler, M. Gannon, K. Sicchio, A Brief History of Wearables, in: Crafting
Wearables, Springer, 2016, pp. 3–10.
[63] Unique Watch Guide, Calculator watches, 2015, [Online] http://www.
uniquewatchguide.com/calculator-watches.html (Accessed March 3, 2021).
[64] R. Bensene, Hewlett Packard HP-01 Calculator Wristwatch, 2019, [Online]
https://www.oldcalculatormuseum.com/hp-01.html (Accessed March 3, 2021).
[65] MoHPC, The Museum of HP Calculators: HP-01, 2019, [Online] https://www.
hpmuseum.org/hp01.htm (Accessed March 3, 2021).
[66] K.A. Popat, P. Sharma, Wearable Computer Applications a Future Perspective,
Int. J. Eng. Innov. Technol. 3 (1) (2013) 213–217.
[67] B. Harrison, Design Moment: Sony Walkman, 1979: The Silver and Blue Portable
Personal Stereo Sold beyond All Expectations, The Irish Times, 1979, [On-
line] https://www.irishtimes.com/life-and-style/homes-and-property/interiors/
design-moment-sony-walkman-1979-1.3465629 (Accessed March 3, 2021).
[68] S. Mann, J. Fung, C. Aimone, A. Sehgal, D. Chen, Designing EyeTap Digital
Eyeglasses for Continuous Lifelong Capture and Sharing of Personal Experiences,
2005.
[69] O. Peltola, Introduction to Wearable Healthcare Technology (Master’s thesis),
Juväskylän Yliopisto, Faculty of Information Technology, 2017.
[70] Tech Blog, Before Smartwatches There was the Seiko UC-2000 Wrist Computer,
2015, [Online] https://www.dailymail.co.uk/sciencetech/article-2584437/Is-
wearable-computer-300-year-old-Chinese-abacus-ring-used-Qing-Dynasty-
help-traders.html (Accessed March 3, 2021).
[71] Polygon, A Visual Guide to Watch Gaming’s 40-year History, 2019, [On-
line] https://www.polygon.com/a/smartwatch-history-guide-evolution/watch-
timeline (Accessed March 3, 2021).
[72] J. Peddie, Augmented Reality: Where We Will All Live, Springer, 2017.
[73] R. Want, A. Hopper, V. Falcão, J. Gibbons, The Active Badge Location System,
ACM Trans. Inf. Syst. 10 (1) (1992) 91–102, http://dx.doi.org/10.1145/128756.
128759.
[74] D. Greaves, Olivetti research active badge, 2010, [Online] http://koo.corpus.
cam.ac.uk/projects/badges/index.html (Accessed March 3, 2021).
[75] O. Amft, P. Lukowicz, From Backpacks to Smartphones: Past, Present, and
Future of Wearable Computers, IEEE Pervas. Comput. 8 (3) (2009) 8–13.
[76] S. Feiner, B. Macintyre, D. Seligmann, Knowledge-Based Augmented Reality,
Commun. ACM 36 (7) (1993) 53–62.
[77] M. Lamming, M. Flynn, Forget-me-Not: Intimate Computing in Support of
Human Memory, in: Proc. of International Symposyum on Next Generation
Human Interface, 1994, p. 4.
[78] D. Knight, A history of palm part 2: Palm PDAs phones 1996 to 2003,
2017, [Online] https://lowendmac.com/2016/a-history-of-palm-part-2-palm-
pdas-and-phones-1996-to-2003/ (Accessed March 3, 2021).
[79] D. Papadopoulos, MBracelet (1999): New York, New York, USA & Lon-
don, UK with the Knowledge Lab, NCR, 2019, [Online] http://www.
fashionabletechnology.org/press/photosbook/hi-res/ft-book-p117.pdf (Accessed
March 3, 2021).
[80] J.-H. Kim, A Study on the Characteristics of Modern Fashion Design for Digital
Nomadic Culture, Fash. Text. Res. J. 9 (1) (2007) 6–14.
[81] Plantronics, An Industry Pioneer Reflects on a Decade’S Worth of Achievements
To Honour the 10th Anniversary of Bluetooth Headsets, 2010, [Online]
https://newsroom.poly.com/press-release/consumer/plantronics-celebrates-10-
years-bluetooth-headset-innovation (Accessed March 3, 2021).
[82] J. McHugh, Wrist-Top Revolution, 2001, [Online] https://www.wired.com/
2003/04/fossil/ (Accessed March 3, 2021).
[83] C. Evers, Researching Action Sport with a GoPro Camera: An Embodied and
Emotional Mobile Video Tale of the Sea, Masculinity and Men-Who-Surf, in:
Researching Embodied Sport, Routledge, 2015, pp. 145–162.
```

```
Computer Networks 193 (2021) 108074
```
[84] S. Shoul, Nike and Apple Team Up To Launch Nike+iPod, 2006, [On-
line] https://www.apple.com/newsroom/2006/05/23nike-and-apple-team-up-
to-launch-nike-ipod/ (Accessed March 3, 2021).
[85] G. Marshall, the Story of Fitbit: How a Wooden Box Became a $4 Billion
Company, 2016, [Online] https://www.wareable.com/fitbit/youre-fitbit-and-
you-know-it-how-a-wooden-box-became-a-dollar-4-billion-company (Accessed
March 3, 2021).
[86] OKTRACKME, Fitbit Wireless Activity and Sleep Tracker, 2013, [Online] [http:](http:)
//oktrackme.com/fitness-tracking/fitbit/ (Accessed March 3, 2021).
[87] Inc. Media Genesis, Watch Out: A Timely History of the Smartwatch, 2019, [On-
line] https://mediag.com/blog/watch-out-a-timely-history-of-the-smartwatch/
(Accessed March 3, 2021).
[88] F. Graham, Samsung S9110 Watch Phone Lets Our Wrists Do the Talking,
2009, [Online] https://www.cnet.com/news/samsung-s9110-watch-phone-lets-
our-wrists-do-the-talking/ (Accessed March 3, 2021).
[89] T. Jowitt, Tales in Tech History: Pebble Smartwatch, 2017, [Online] https://
[http://www.silicon.co.uk/mobility/tales-tech-history-pebble-smartwatch-220973](http://www.silicon.co.uk/mobility/tales-tech-history-pebble-smartwatch-220973) (Ac-
cessed March 3, 2021).
[90] C. Steele, A Look Back At Pebble’S Rise and Fall, 2016, [Online]
https://web.archive.org/web/20170718150503/https://www.pcmag.com/
article/350161/a-look-back-at-pebbles-rise-and-fall (Accessed March 3, 2021).
[91] PBC Kickstarter, Pebble: E-Paper Watch for iPhone and Android, 2012,
[Online] https://www.kickstarter.com/projects/getpebble/pebble-e-paper-
watch-for-iphone-and-android (Accessed March 3, 2021).
[92] E. Betters, Google Glass: A Brief History, 2015, [Online] https://www.pocket-
lint.com/ar-vr/news/google/132399-google-glass-a-brief-history (Accessed
March 3, 2021).
[93] E. Mack, Confirmed: Google Glass Arrives in 2013, and under $1, 500, 2013,
[Online] https://www.cnet.com/news/confirmed-google-glass-arrives-in-2013-
and-under-1500/ (Accessed March 3, 2021).
[94] 6 Pack Fitness, Best Fitness Trackers: Top 5 Fitness BandS of 2014, 2014,
[Online] https://www.sixpackbags.com/blogs/news/fitness-b{and}s (Accessed
March 3, 2021).
[95] M. Nguyen, The Most Successful Wearables for Consumers, 2016, [Online]
https://www.wearable-technologies.com/2016/01/the-most-successful-
wearables-for-consumers/ (Accessed March 3, 2021).
[96] M. Starr, Tommy Hilfiger Launches Solar Power Jackets To Charge Your
Phone, 2014, [Online] https://www.cnet.com/news/tommy-hilfiger-launches-
solar-power-jackets-to-charge-your-phone/ (Accessed March 3, 2021).
[97] D. D’Orazio, Google Reveals Android Wear, an Operating System for
Smartwatches, 2014, [Online] https://www.theverge.com/2014/3/18/
5522226/google-reveals-android-wear-an-operating-system-designed-for
(Accessed March 3, 2021).
[98] T. Bajarin, The Real Reason Apple Made the Apple Watch, TIME, 2016, [Online]
https://time.com/4323318/apple-watch-steve-jobs-health/ (Accessed March 3,
2021).
[99] K.-J. Brickwood, G. Watson, J. O’Brien, a.D. Williams, Consumer-Based Wear-
able Activity Trackers Increase Physical Activity Participation: Systematic
Review and Meta-Analysis, JMIR MHealth and UHealth 7 (4) (2019) e11819.
[100] C. Attig, T. Franke, I. Track, I Track Therefore I Walk–Exploring the Motiva-
tional Costs of Wearing Activity Trackers in Actual Users, Int. J. Hum.-Comput.
Stud. 127 (2019) 211–224.
[101] E. Olshannikova, A. Ometov, Y. Koucheryavy, Towards Big Data Visualiza-
tion for Augmented Reality, in: Proc. of IEEE 16th Conference on Business
Informatics, Vol. 2, IEEE, 2014, pp. 33–37.
[102] M.C. Tom Dieck, T.H. Jung, D. Tom Dieck, Enhancing Art Gallery Visitors’
Learning Experience using Wearable Augmented Reality: Generic Learning
Outcomes Perspective, Curr. Issues Tour. 21 (17) (2018) 2014–2034.
[103] I.P. Tussyadiah, T.H. Jung, M.C. Tom Dieck, Embodiment of Wearable Aug-
mented Reality Technology in Tourism Experiences, J. Travel Res. 57 (5) (2018)
597–611.
[104] S.K. Ong, A.Y.C. Nee, Virtual and Augmented Reality Applications in
Manufacturing, Springer Science & Business Media, 2013.
[105] S. Alkhalifa, M. Al-Razgan, Enssat: Wearable Technology Application for
the Deaf and Hard of Hearing, Multimedia Tools Appl. 77 (17) (2018)
22007–22031.
[106] S.-N. Yao, Headphone-Based Immersive Audio for Virtual Reality Headsets, IEEE
Trans. Consum. Electron. 63 (3) (2017) 300–308.
[107] M.L. Hammock, a. Chortos, B.C.-K. Tee, J.B.-H. Tok, Z. Bao, 25th Anniversary
Article: The Evolution of Electronic Skin (E-Skin): A Brief History, Design
Considerations, and Recent Progress, Adv. Mater. 25 (42) (2013) 5997–6038.
[108] S. Gong, D.T. Lai, B. Su, K.J. Si, Z. Ma, L.W. Yap, P. Guo, W. Cheng,
Highly Stretchy Black Gold E-Skin Nanopatches As Highly Sensitive Wearable
Biomedical Sensors, Adv. Electron. Mater. 1 (4) (2015) 1400063.
[109] R. Dahiya, N. Yogeswaran, F. Liu, L. Manjakkal, E. Burdet, V. Hayward, H.
JÖRntell, Large-Area Soft E-Skin: The Challenges beyond Sensor Designs, Proc.
IEEE 107 (10) (2019) 2016–2033.
[110] a. Komolafe, R. Torah, Y. Wei, H. Nunes-Matos, M. Li, D. Hardy, T. Dias, M. Tu-
dor, S. Beeby, Integrating Flexible Filament Circuits for E-Textile Applications,
Adv. Mater. Technol. 4 (7) (2019) 1900176.

```
[111] L.M. Castano, a.B. Flatau, Smart Fabric Sensors and E-Textile Technologies: A
Review, Smart Mater. Struct. 23 (5) (2014) 053001.
[112] S. Imani, a.J. BandOdkar, a.V. Mohan, R. Kumar, S. Yu, J. Wang, P.P.
Mercier, A Wearable Chemical–Electrophysiological Hybrid Biosensing System
for Real-Time Health and Fitness Monitoring, Nature Commun. 7 (1) (2016)
1–7.
[113] C.-T. Lin, C.-H. Chuang, Z. Cao, a.K. Singh, C.-S. Hung, Y.-H. Yu, M. Nascimben,
Y.-T. Liu, J.-T. King, T.-P. Su, Others, Forehead EEG in Support of Future Fea-
sible Personal Healthcare Solutions: Sleep Management, Headache Prevention,
and Depression Treatment, IEEE Access 5 (2017) 10612–10621.
[114] J.L. Park, M.M. Fairweather, D.I. Donaldson, Making the Case for Mobile
Cognition: EEG and Sports Performance, Neurosci. Biobehav. Rev. 52 (2015)
117–130.
[115] C. Pittman, J.J. LaViola Jr, Exploring Head Tracked Head Mounted Displays for
First Person Robot Teleoperation, in: Proc. of the 19th International Conference
on Intelligent User Interfaces, 2014, pp. 323–328.
[116] E. Taylor, Lights, Camera, Redaction... Police Body-Worn Cameras; Autonomy,
Discretion and Accountability, Surveill. Soc. 14 (1) (2016) 128–132.
[117] R. Pirmagomedov, D. Moltchanov, a. Ometov, K. Muhammad, S. Andreev,
Y. Koucheryavy, Facilitating MmWave Mesh Reliability in PPDR Scenarios
Utilizing Artificial Intelligence, IEEE Access 7 (2019) 180700–180712.
[118] Teslasuit, Full Body Haptic VR Suite, 2019, [Online] https://teslasuit.io
(Accessed March 3, 2021).
[119] R.W. Lindeman, R. Page, Y. Yanagida, J.L. Sibert, Towards Full-Body Haptic
Feedback: The Design and Deployment of a Satialized Vibrotactile Fedback Sys-
tem, in: Proc. of ACM Symposium on Virtual Reality Software and Technology,
2004, pp. 146–149.
[120] A. Al Maimani, A. Roudaut, Frozen Suit: Designing a Changeable Stiffness Sit
and Its Application to haptic Games, in: Proc. of CHI Conference on Human
Factors in Computing Systems, 2017, pp. 2440–2448.
[121] K. Antonakoglou, X. Xu, E. Steinbach, T. Mahmoodi, M. Dohler, Toward Haptic
Communications over the 5G Tactile Internet, IEEE Commun. Surv. Tutor. 20
(4) (2018) 3034–3059.
[122] A.M. Okamura, Haptic Feedback in Robot-Assisted Minimally Invasive Surgery,
Curr. Opin. Urol. 19 (1) (2009) 102.
[123] S. Pradhan, The Present and Future of Ingestible Sensors – the New Taste
of Science, 2019, [Online] https://www.prescouter.com/2019/01/ingestible-
sensors-innovations/ (Accessed March 3, 2021).
[124] A.S. Barbone, M. Meftah, K. Markiewicz, K. Dellimore, Beyond Wearables and
Implantables: A Scoping Review of Insertable Medical Devices, Biomed. Phys.
Eng. Express 5 (6) (2019) 062002.
[125] L.M. Ni, Y. Liu, Y.C. Lau, A.P. Patil, LANDMARC: Indoor Location Sensing using
Active RFID, in: Proc. of 1st International Conference on Pervasive Computing
and Communications (PERCOM), IEEE, 2003, pp. 407–415.
[126] J. Ting, A. Del Vecchio, D. Friedenberg, M. Liu, C. Schoenewald, D. Sarma,
J. Collinger, S. Colachis, G. Sharma, D. Farina, et al., A Wearable Neural
Interface for Detecting and Decoding Attempted Hand Movements in a Person
with Tetraplegia, in: Proc. of 41st Annual International Conference of the
IEEE Engineering in Medicine and Biology Society (EMBC), IEEE, 2019, pp.
1930–1933.
[127] A. Cutrone, S. Micera, Implantable Neural Interfaces and Wearable Tactile
Systems for Bidirectional Neuroprosthetics Systems, Adv. Healthc. Mater. 8 (24)
(2019) 1801345.
[128] M. Chae, K. Chen, W. Liu, J. Kim, M. Sivaprakasam, A 4-Channel Wearable
Wireless Neural Recording System, in: Proc. of IEEE International Symposium
on Circuits and Systems, IEEE, 2008, pp. 1760–1763.
[129] L.-D. Liao, C.-Y. Chen, I.-J. Wang, S.-F. Chen, S.-Y. Li, B.-W. Chen, J.-Y. Chang,
C.-T. Lin, Gaming Control using a Wearable and Wireless EEG-Based Brain-
Computer Interface Device with Novel Dry Foam-Based Sensors, J. Neuroeng.
Rehabil. 9 (1) (2012) 5.
[130] G. Cattan, C. Mendoza, a. Andreev, M. Congedo, Recommendations for Integrat-
ing a P300-Based Brain Computer Interface in Virtual Reality Environments for
Gaming, Computers 7 (2) (2018) 34.
[131] S. Draper, 4 Smart Sleep Masks To Help You Get Some Sleep While
on the Go, Wearable Technologies International, 2019, [Online]
https://www.wearable-technologies.com/2019/07/the-4-best-smart-sleep-
masks-to-help-you-get-some-sleep-while-on-the-go/ (Accessed March 3, 2021).
[132] Silentmode’S PowerMask Is a $200 Connected Relaxation Mask, 2021,
[Online] https://techcrunch.com/2018/11/23/silentmodes-powermask-is-a-
200-connected-relaxation-mask/ (Accessed March 3, 2021).
[133] Ripple Safety, The Revolutionary Safety Button, 2019, [Online] https://
ripplesafety.com(Accessed March 3, 2021).
[134] J. Patel, R. Hasan, Smart Bracelets: Towards Automating Personal Safety
using Wearable Smart Jewelry, in: Proc. of 15th IEEE Annual Consumer
Communications & Networking Conference (CCNC), IEEE, 2018, pp. 1–2.
[135] A. Ferrone, F. Maita, L. Maiolo, M. Arquilla, A. Castiello, A. Pecora, X. Jiang,
C. Menon, L. Colace, Wearable Band for Hand Gesture Recognition Based on
Strain Sensors, in: Proc. of 6th IEEE International Conference on Biomedical
Robotics and Biomechatronics (BioRob), IEEE, 2016, pp. 1319–1322.
```

```
Computer Networks 193 (2021) 108074
```
[136] H. Liu, L. Wang, Robot Collaboration, Gesture Recognition for Human-: A
Review, Int. J. Ind. Ergon. 68 (2018) 355–367.
[137] Z. Yang, Q. Zhou, L. Lei, K. Zheng, W. Xiang, An IoT-Cloud Based Wearable
ECG Monitoring System for Smart Healthcare, J. Med. Syst. 40 (12) (2016)
286.
[138] M. Zubair, C. Yoon, H. Kim, J. Kim, J. Kim, Smart Wearable Band for Stress
Detection, in: Proc. of 5th International Conference on IT Convergence and
Security (ICITCS), IEEE, 2015, pp. 1–4.
[139] NEOFECT, Smart Glove for Hand Rehabilitation, 2016, [Online] https://www.
neofect.com/en/ (Accessed March 3, 2021).
[140] M. Zhu, Z. Sun, Z. Zhang, Q. Shi, T. He, H. Liu, T. Chen, C. Lee, Haptic-
Feedback Smart Glove As a Creative Human-Machine Interface (HMI) for
Virtual/Augmented Reality Applications, Sci. Adv. 6 (19) (2020) eaaz8693.
[141] GadgetFlow, The World’S First Heated Jacket Managed By Smartphone,
2016, [Online] https://thegadgetflow.com/portfolio/worlds-first-heated-jacket-
managed-smartphone/ (Accessed March 3, 2021).
[142] J. Park, J. Kim, S.-Y. Kim, W.H. Cheong, J. Jang, Y.-G. Park, K. Na, Y.-T.
Kim, J.H. Heo, C.Y. Lee, et al., Soft, Smart Contact Lenses with Integrations of
Wireless Circuits, Glucose Sensors, and Displays, Sci. Adv. 4 (1) (2018) 9841.
[143] J. Kim, M. Kim, M.-S. Lee, K. Kim, S. Ji, Y.-T. Kim, J. Park, K. Na, K.-H. Bae,
H.K. Kim, Others, Wearable Smart Sensor Systems Integrated on Soft Contact
Lenses for Wireless Ocular Diagnostics, 2017.
[144] B. Pellegrini, C. Zoppirolli, L. Bortolan, P. Zamparo, F. Schena, Gait Models
and Mechanical Energy in Three Cross-Country Skiing Techniques, J. Exp. Biol.
217 (21) (2014) 3910–3918.
[145] F. Laamarti, F. Arafsha, B. Hafidh, A. El Saddik, Automated Athlete Hap-
tic Training System for Soccer Sprinting, in: Proc. of IEEE Conference on
Multimedia Information Processing and Retrieval (MIPR), IEEE, 2019, pp.
303–309.
[146] Cheeky Rascals, Know Your Baby Is Okay: The Owlet Smart Sock Tracks Your
Baby’s Heart Rate and Oxygen Levels, 2019, [Online] https://owletbabycare.
co.uk (Accessed March 3, 2021).
[147] H. Witt, T. Nicolai, H. Kenn, Designing a Wearable User Interface for
HandS-Free Interaction in Maintenance Applications, in: Proc. of IEEE Inter-
national Conference on Pervasive Computing and Communications Workshops
(PERCOMW’06), IEEE, 2006, pp. 4–pp.
[148] B. Heater, Neofect’s Powered Glove for People with Paralysis is Shipping
this Summer, 2019, [Online] https://techcrunch.com/2019/01/07/neofects-
powered-glove-for-people-with-paralysis-is-shipping-this-summer/ (Accessed
March 3, 2021).
[149] J. Blake, H.B. Gurocak, Haptic Glove with MR Brakes for Virtual Reality,
IEEE/ASME Trans. Mechatronics 14 (5) (2009) 606–615.
[150] F. El-Amrawy, M.I. Nounou, Are Currently Available Wearable Devices for
Activity Tracking and Heart Rate Monitoring Accurate, Precise, and Medically
Beneficial?, Healthc. Inform. Res. 21 (4) (2015) 315–320.
[151] H. Kalantarian, N. Alshurafa, T. Le, M. Sarrafzadeh, Non-invasive Detection of
Medication Adherence Using a Digital Smart Necklace, in: Proc. of IEEE Inter-
national Conference on Pervasive Computing and Communication Workshops
(PerCom Workshops), IEEE, 2015, pp. 348–353.
[152] N. Alshurafa, H. Kalantarian, M. Pourhomayoun, J.J. Liu, S. Sarin, B. Shahbazi,
M. Sarrafzadeh, Recognition of Nutrition Intake Using Time-Frequency Decom-
position in a Wearable Necklace Using a Piezoelectric Sensor, IEEE Sens. J. 15
(7) (2015) 3909–3916.
[153] Opter Life Inc., The Smart Posture Necklace: Correct Your Posture. Track Your
Activity, Sleep, UV Exposure, and More, 2019, [Online] https://opterlife.com/
(Accessed March 3, 2021).
[154] V. Hyndavi, N.S. Nikhita, S. Rakesh, Smart Wearable Device for Women Safety
Using IoT, in: Proc. of 5th International Conference on Communication and
Electronics Systems (ICCES), IEEE, 2020, pp. 459–463.
[155] S. Draper, Wearable Ultrasound Patch Monitors Blood Pressure in Deep Arteries,
2019, [Online] https://www.wearable-technologies.com/2018/11/wearable-
ultrasound-patch-monitors-blood-pressure-in-deep-arteries/ (Accessed March 3,
2021).
[156] M. Klum, M. Urban, T. Tigges, A.-G. Pielmus, A. Feldheiser, T. Schmitt, R.
Orglmeister, Wearable Cardiorespiratory Monitoring Employing a Multimodal
Digital Patch Stethoscope: Estimation of ECG, PEP, LVETand Respiration Using
a 55 mm Single-Lead ECG and Phonocardiogram, Sensors 20 (7) (2020) 2033.
[157] C. Russey, These Smart Patches Monitor Your Stress to Help You
Lead a Happier, Healthier Life, 2018, [Online] https://www.wearable-
technologies.com/2018/11/these-smart-patches-monitor-your-stress-to-help-
you-lead-a-happier-healthier-life/ (Accessed March 3, 2021).
[158] R. Long, M. McShane, Optical Instrument Design for Interrogation of Dermally-
Implanted Luminescent Microparticle Sensors, in: Proc. of 30th Annual
International Conference of the IEEE Engineering in Medicine and Biology
Society, IEEE, 2008, pp. 5656–5659.
[159] D. Meetoo, L. Wong, B. Ochieng, Smart Tattoo: Technology for Monitoring
Blood Glucose in the Future, Br. J. Nurs. 28 (2) (2019) 110–115.
[160] D. Pal, A. Tassanaviboon, C. Arpnikanondt, B. Papasratorn, Quality of Experi-
ence of Smart-Wearables: From Fitness-Bands to Smartwatches, IEEE Consum.
Electron. Mag. 9 (1) (2019) 49–53.

```
[161] E. Olshannikova, A. Ometov, Y. Koucheryavy, T. Olsson, Visualizing Big Data
with Augmented and Virtual Reality: Challenges and Research Agenda, J Big
Data 2 (1) (2015) 22.
[162] C. Fertleman, P. Aubugeau-Williams, C. Sher, A.-N. Lim, S. Lumley, S. Delacroix,
X. Pan, A Discussion of Virtual Reality as a New Tool for Training Healthcare
Professionals, Front. Public Health 6 (2018) 44.
[163] P. Milgram, F. Kishino, A Taxonomy of Mixed Reality Visual Displays, IEICE
Trans. Inf. Syst. 77 (12) (1994) 1321–1329.
[164] Å. Fast-Berglund, L. Gong, D. Li, Testing and Validating Extended Reality (XR)
Technologies in Manufacturing, Proc. Manuf. 25 (2018) 31–38.
[165] C. Andrews, M.K. Southworth, J.N. Silva, J.R. Silva, Extended Reality in Medical
Practice, Curr. Treat. Options Cardiovasc. Med. 21 (4) (2019) 18.
[166] W. Hoenig, C. Milanes, L. Scaria, T. Phan, M. Bolas, N. Ayanian, Mixed Reality
for Robotics, in: Proc. of IEEE/RSJ International Conference on Intelligent
Robots and Systems (IROS), IEEE, 2015, pp. 5382–5387.
[167] N. Kolokas, S. Krinidis, A. Drosou, D. Ioannidis, D. Tzovaras, Gait Matching
by Mapping Wearable to Camera Privacy-Preserving Recordings: Experimental
Comparison of Multiple Settings, in: Proc. of 6th International Conference
on Control, Decision and Information Technologies (CoDIT), IEEE, 2019, pp.
338–343.
[168] M.S. Mahmud, H. Fang, H. Wang, An Integrated Wearable Sensor for Unob-
trusive Continuous Measurement of Autonomic Nervous System, IEEE Internet
Things J. 6 (1) (2018) 1104–1113.
[169] M. Xu, F. Qian, M. Zhu, F. Huang, S. Pushp, X. Liu, Deepwear: Adaptive Local
Offloading for on-Wearable Deep Learning, IEEE Trans. Mob. Comput. 19 (2)
(2019) 314–330.
[170] A.D. Cheok, W. Weihua, X. Yang, S. Prince, F.S. Wan, M. Billinghurst, H. Kato,
Interactive Theatre Experience in Embodied+ Wearable Mixed Reality Space,
in: Proc. of International Symposium on Mixed and Augmented Reality, IEEE,
2002, pp. 59–317.
[171] M. Golkarifard, J. Yang, Z. Huang, A. Movaghar, P. Hui, Dandelion: A Unified
Code Offloading System for Wearable Computing, IEEE Trans. Mob. Comput.
18 (3) (2018) 546–559.
[172] H.-J. Hong, C.-L. Fan, Y.-C. Lin, C.-H. Hsu, Optimizing Cloud-based Video
Crowdsensing, IEEE Internet Things J. 3 (3) (2016) 299–313.
[173] Is Lithium-Ion the Ideal Battery?, 2021, [Online] Available: https://
batteryuniversity.com/learn/archive/is_lithium_ion_the_ideal_battery (Accessed
March 3, 2021).
[174] Lithium coin cells, 2021, [Online] Available: https://www.microbattery.com/
coin-cells (Accessed March 3, 2021).
[175] Lithium-ion vs lithium-polymer: what’s the difference?, 2021, [Online]
Available: https://www.androidauthority.com/lithium-ion-vs-lithium-polymer-
whats-the-difference-27608/ (Accessed March 3, 2021).
[176] R. Carroll, R. Cnossen, M. Schnell, D. Simons, Continua: An Interoperable
Personal Healthcare Ecosystem, IEEE Pervas. Comput. 6 (4) (2007) 90–94.
[177] M. Magno, L. Benini, C. Spagnol, E. Popovici, Wearable Low Power Dry Surface
Wireless Sensor Node for Healthcare Monitoring Application, in: Proc. of IEEE
9th International Conference on Wireless and Mobile Computing, Networking
and Communications (WiMob), IEEE, 2013, pp. 189–195.
[178] M.C. Domingo, An Overview of the Internet of Things for People with
Disabilities, J. Netw. Comput. Appl. 35 (2) (2012) 584–596.
[179] R. Djapic, G. Vivier, B. Zhen, J. Wang, J. Lee, W. Haiming, Wearables White
Paper, White paper, TNO etc, 2018.
[180] F. Delmastro, V. Arnaboldi, M. Conti, People-Centric Computing and
Communications in Smart Cities, IEEE Commun. Mag. 54 (7) (2016) 122–128.
[181] C. Mouradian, D. Naboulsi, S. Yangui, R.H. Glitho, M.J. Morrow, P.A. Polakos,
A Comprehensive Survey on Fog Computing: State-of-the-Art and Research
Challenges, IEEE Commun. Surv. Tutor. 20 (1).
[182] P. Vilela, J. Rodrigues, R. Righi, S. Kozlov, V. Rodrigues, Looking at Fog
Computing for e-Health through the Lens of Deployment Challenges and
Applications, Sensors (20).
[183] F. Kraemer, A. Bråten, N. Tamkittikhun, D. Palma, Fog computing in healthcare
```
- a review and discussion, IEEE Access PP (2017) 9206–9222, [http://dx.doi.](http://dx.doi.)
org/10.1109/ACCESS.2017.2704100.
[184] F. Bonomi, R. Milito, J. Zhu, S. Addepalli, Fog computing and its role in the
internet of things, in: Proceedings of the First Edition of the MCC Workshop on
Mobile Cloud Computing, MCC ’12, Association for Computing Machinery, New
York, NY, USA, 2012, pp. 13–16, [http://dx.doi.org/10.1145/2342509.2342513.](http://dx.doi.org/10.1145/2342509.2342513.)
[185] F. Bonomi, R. Milito, P. Natarajan, J. Zhu, Fog Computing: A Platform for
Internet of Things and Analytics, Springer International Publishing, Cham, 2014,
pp. 169–186, [http://dx.doi.org/10.1007/978-3-319-05029-4_7.](http://dx.doi.org/10.1007/978-3-319-05029-4_7.)
[186] ZIGURAT Innovation School, Exploring beyond cloud fog & edge computing –
innovation blog, 2020, [Online] https://www.e-zigurat.com/innovation-school/
blog/beyond-cloud-fog-edge-computing/#comments (Accessed March 3, 2021).
[187] A. Yousefpour, C. Fung, T. Nguyen, K. Kadiyala, F. Jalali, A. Niakanlahiji, J.
Kong, J.P. Jue, All One Needs to Know about Fog Computing and Related Edge
Computing Paradigms: A Complete Survey, J. Syst. Archit. 98 (2019) 289–330.
[188] J. Ren, D. Zhang, S. He, Y. Zhang, T. Li, A Survey on End-Edge-Cloud
Orchestrated Network Computing Paradigms: Transparent Computing, Mobile
Edge Computing, Fog Computing, and Cloudlet, ACM Comput. Surv. 52 (6)
(2019) 1–36.


```
Computer Networks 193 (2021) 108074
```
[189] K. Dolui, S.K. Datta, Comparison of Edge Computing Implementations: Fog
Computing, Cloudlet and Mobile Edge Computing, in: Proc. of Global Internet
of Things Summit (GIoTS), IEEE, 2017, pp. 1–6.
[190] A. Rubin, J. Ophoff, nvestigating Adoption Factors of Wearable Technology in
Health and Fitness, in: Proc. of Open Innovations Conference (OI), 2018, pp.
176–186.
[191] H. Cao, M. Brown, L. Chen, R. Smith, M. Wachowicz, Lessons Learned from
Integrating Batch and Stream Processing Using IoT Data, in: Proc. of 6th
International Conference on Internet of Things: Systems, Management and
Security (IOTSMS), 2019, pp. 32–34.
[192] M. Obalı, B. Dursun, Z. Erdem, A.K. Görür, A Real Time Data Ware-
house Approach for Data Processing, in: Proc. of 21st Signal Processing and
Communications Applications Conference (SIU), 2013, pp. 1–4.
[193] T. Abughofa, F. Zulkernine, Towards Online Graph Processing with Spark
Streaming, in: Proc. of IEEE International Conference on Big Data (Big Data),
2017, pp. 2787–2794.
[194] M. Terzi, A. Cenedese, G. Susto, A Multivariate Symbolic Approach to Activ-
ity Recognition for Wearable Applications, IFAC-PapersOnLine 50 (1) (2017)
15865–15870.
[195] Q. Wen, L. Sun, X. Song, J. Gao, X. Wang, H. Xu, Time Series Data
Augmentation for Deep Learning: A Survey, arXiv preprint arXiv:2002.12478.
[196] Z. Hussain, Q.Z. Sheng, W.E. Zhang, A Review and Categorization of Techniques
on Device-Free Human Activity Recognition, J. Netw. Comput. Appl. (2020)
102738.
[197] L.M. Dang, K. Min, H. Wang, M.J. Piran, C.H. Lee, H. Moon, Sensor-Based and
Vision-Based Human Activity Recognition: A Comprehensive Survey, Pattern
Recognit. 108 (2020) 107561.
[198] S. Pardoel, J. Kofman, J. Nantel, E.D. Lemaire, Wearable-Sensor-Based Detection
and Prediction of Freezing of Gait in Parkinson’s Disease: A Review, Sensors
19 (23) (2019) 5141.
[199] M. Zhang, Z. Cui, M. Neumann, Y. Chen, An End-to-End Deep Learning
Architecture for Graph Classification, in: Proc. of 32nd AAAI Conference on
Artificial Intelligence, 2018.
[200] J. Guo, L. Yang, R. Bie, J. Yu, Y. Gao, Y. Shen, A. Kos, An XGBoost-
Based Physical Fitness Evaluation Model Using Advanced Feature Selection
and Bayesian Hyper-Parameter Optimization for Wearable Running Monitoring,
Comput. Netw. 151 (2019) 166–180.
[201] F.J. Ordóñez, D. Roggen, Deep Convolutional and lstm Recurrent Neural
Networks for Multimodal Wearable Activity Recognition, Sensors 16 (1) (2016)
115.
[202] A.A. Aljarrah, A.H. Ali, Human Activity Recognition using PCA and BiL-
STM Recurrent Neural Networks, in: Proc. of 2nd International Conference
on Engineering Technology and Its Applications (IICETA), IEEE, 2019, pp.
156–160.
[203] L. Eren, T. Ince, S. Kiranyaz, A Generic Intelligent Bearing Fault Diagnosis
System Using Compact Adaptive 1D CNN Classifier, J. Signal Process. Syst. 91
(2) (2019) 179–189.
[204] F. Samie, L. Bauer, J. Henkel, IoT Technologies for Embedded Computing: A
Survey, in: Proc. of International Conference on Hardware/Software Codesign
and System Synthesis (CODES+ ISSS), IEEE, 2016, pp. 1–10.
[205] E. Ferro, F. Potorti, Bluetooth and Wi-Fi Wireless Protocols: A Survey and a
Comparison, IEEE Wirel. Commun. 12 (1) (2005) 12–26.
[206] A. Ometov, E. Olshannikova, P. Masek, T. Olsson, J. Hosek, S. Andreev, Y.
Koucheryavy, Dynamic Trust Associations over Socially-Aware D2D Technology:
A Practical Implementation Perspective, IEEE Access 4 (2016) 7692–7702.
[207] Y. Ghasempour, C.R. da Silva, C. Cordeiro, E.W. Knightly, 802.11ay: Next-
Generation 60 GHz Communication for 100 GB/s Wi-Fi, IEEE Commun. Mag.
55 (12) (2017) 186–192.
[208] M.S. Elbamby, C. Perfecto, M. Bennis, K. Doppler, Toward Low-Latency and
Ultra-Reliable Virtual Reality, IEEE Netw. 32 (2) (2018) 78–84.
[209] D. Solomitckii, V. Semkin, R. Naderpour, A. Ometov, S. Andreev, Comparative
Evaluation of Radio Propagation Properties at 15 GHz and 60 GHz Frequencies,
in: Proc. of 9th International Congress on Ultra Modern Telecommunications
and Control Systems and Workshops (ICUMT), IEEE, 2017, pp. 91–95.
[210] H. Elayan, O. Amin, B. Shihada, R.M. Shubair, M.-S. Alouini, Terahertz Band:
The Last Piece of RF Spectrum Puzzle for Communication Systems, IEEE Open
J. Commun. Soc. 1 (2019) 1–32.
[211] P.H. Pathak, X. Feng, P. Hu, P. Mohapatra, Visible Light Communication,
Networking, and Sensing: A Survey, Potential and Challenges, IEEE Commun.
Surv. Tutor. 17 (4) (2015) 2047–2077.
[212] R. Bridgelall, Wearable RFID reader and system, 2006.
[213] V. Coskun, B. Ozdenizci, K. Ok, A Survey on Near Field Communication (NFC)
Technology, Wirel. Pers. Commun. 71 (3) (2013) 2259–2294.
[214] H. Sun, Z. Zhang, R.Q. Hu, Y. Qian, Wearable Communications in 5G:
Challenges and Enabling Technologies, IEEE Veh. Technol. Mag. 13 (3) (2018)
100–109.
[215] C. Orfanidis, K. Dimitrakopoulos, X. Fafoutis, M. Jacobsson, Towards Battery-
Free LPWAN Wearables, in: Proc. of 7th International Workshop on Energy
Harvesting & Energy-Neutral Sensing Systems, 2019, pp. 52–53.

```
[216] P.A. Catherwood, J. Rafferty, S. McComb, J. McLaughlin, LPWAN Wearable
Intelligent Healthcare Monitoring for Heart Failure Prevention, in: Proc. of 32nd
International BCS Human Computer Interaction Conference Vol. 32, 2018, pp.
1–4.
[217] R. Fernández-Garcia, I. Gil, An Alternative Wearable Tracking System Based on
a Low-Power Wide-Area Network, Sensors 17 (3) (2017) 592.
[218] Y. Hao, Y. Jiang, M.S. Hossain, A. Ghoneim, J. Yang, I. Humar, Data-Driven
Resource Management in a 5G Wearable Network Using Network Slicing
Technology, IEEE Sens. J. 19 (19) (2018) 8379–8386.
[219] Y. Hao, D. Tian, G. Fortino, J. Zhang, I. Humar, Network Slicing Technology
in a 5G Wearable Network, IEEE Commun. Stand. Mag. 2 (1) (2018) 66–71.
[220] Y. Li, L. Sun, W. Wang, Exploring Device-to-Device Communication for
Mobile Cloud Computing, in: Proc. of IEEE International Conference on
Communications (ICC), IEEE, 2014, pp. 2239–2244.
[221] Z. Cheng, P. Li, J. Wang, S. Guo, Just-in-Time Code Offloading for Wearable
Computing, IEEE Trans. Emerg. Top. Comput. 3 (1) (2015) 74–83.
[222] D. Huang, L. Yang, S. Zhang, Dust: Real-time Code Offloading System for
Wearable Computing, in: Proc. of IEEE Global Communications Conference
(GLOBECOM), IEEE, 2015, pp. 1–7.
[223] B. Shi, J. Yang, Z. Huang, P. Hui, Offloading Guidelines for Augmented
Reality Applications on Wearable Devices, in: Proc. of 23rd ACM international
conference on Multimedia, 2015, pp. 1271–1274.
[224] M. Devos, A. Ometov, N. Mäkitalo, T. Aaltonen, S. Andreev, Y. Koucheryavy,
D2D Communications for Mobile Devices: Technology Overview and Prototype
Implementation, in: Proc. of 8th International Congress on Ultra Modern
Telecommunications and Control Systems and Workshops (ICUMT), IEEE, 2016,
pp. 124–129.
[225] Y. Yang, Y. Geng, L. Qiu, W. Hu, G. Cao, Context-Aware Task Offloading
for Wearable Devices, in: Proc. of 26th International Conference on Computer
Communication and Networks (ICCCN), IEEE, 2017, pp. 1–9.
[226] M. Usman, A.A. Gebremariam, U. Raza, F. Granelli, A Software-Defined Device-
to-Device Communication Architecture for Public Safety Applications in 5G
Networks, IEEE Access 3 (2015) 1649–1654.
[227] M.M. Alam, D.B. Arbia, E.B. Hamida, Research Trends in Multi-Standard
Device-to-Device Communication in Wearable Wireless Networks, in: Proc.
of International Conference on Cognitive Radio Oriented Wireless Networks,
Springer, 2015, pp. 735–746.
[228] J. Foerster, J. Lansford, J. Laskar, T. Rappaport, S. Kato, Realizing Gbps Wireless
Personal Area Networks, IEEE J. Sel. Areas Commun. 27 (8) (2009) 1313–1317.
[229] C. Park, T.S. Rappaport, Short-Range Wireless Communications for Next-
Generation Networks: UWB, 60 GHz Millimeter-Wave WPAN, and ZigBee, IEEE
Wirel. Commun. 14 (4) (2007) 70–78.
[230] K. Venugopal, R.W. Heath, Millimeter Wave Networked Wearables in Dense
Indoor Environments, IEEE Access 4 (2016) 1205–1221.
[231] G.H. Sim, A. Loch, A. Asadi, V. Mancuso, J. Widmer, 5G millimeter-Wave and
D2D Symbiosis: 60 GHz for Proximity-based Services, IEEE Wirel. Commun. 24
(4) (2017) 140–145.
[232] Y. Niu, Y. Li, D. Jin, L. Su, A.V. Vasilakos, A Survey of Millimeter Wave
Communications (mmWave) for 5G: Opportunities and Challenges, Wirel. Netw.
21 (8) (2015) 2657–2676.
[233] F.O. Ombongi, H.O. Absaloms, P.L. Kibet, Resource Allocation in Millimeter-
Wave Device-to-Device Networks, Mob. Inf. Syst. (2019).
[234] D. Singh, A. Chattopadhyay, S.C. Ghosh, Distributed Relay Selection in Presence
of Dynamic Obstacles in Millimeter Wave D2D Communication, arXiv preprint
arXiv:1910.14367.
[235] L. Atzori, A. Iera, G. Morabito, M. Nitti, The Social Internet of Things (SIoT)–
When Social Networks Meet the Internet of Things: Concept, Architecture and
Network Characterization, Comput. Netw. 56 (16) (2012) 3594–3608.
[236] M. Roopa, S. Pattar, R. Buyya, K.R. Venugopal, S. Iyengar, L. Patnaik, Social
Internet of Things (SIoT): Foundations, thrust areas, systematic review and
future directions, Comput. Commun. 139 (2019) 32–57.
[237] D. Moltchanov, R. Kovalchukov, M. Gerasimenko, S. Andreev, Y. Koucheryavy,
M. Gerla, Socially Inspired Relaying and Proactive Mode Selection in mmWave
Vehicular Communications, IEEE Internet Things J. 6 (3) (2019) 5172–5183.
[238] S. Pizzi, C. Suraci, A. Iera, A. Molinaro, G. Araniti, A Sidelink-Aided Approach
for Secure Multicast Service Delivery: From Human-Oriented Multimedia Traffic
to Machine Type Communications, IEEE Trans. Broadcast, 2020.
[239] M. Nitti, G.A. Stelea, V. Popescu, M. Fadda, When Social Networks Meet D2D
Communications: A Survey, Sensors 19 (2) (2019) 396.
[240] J. Li, M. Liu, J. Lu, F. Shu, Y. Zhang, S. Bayat, D.N.K. Jayakody, On Social-
Aware Content Caching for D2D-enabled Cellular Networks with Matching
Theory, IEEE Internet Things J. 6 (1) (2017) 297–310.
[241] L. Militano, A. Orsino, G. Araniti, M. Nitti, L. Atzori, A. Iera, Trusted D2D-based
Data Uploading in in-Band narrowband-IoT with Social Awareness, in: Proc. of
27th Annual International Symposium on Personal, Indoor, and Mobile Radio
Communications (PIMRC), IEEE, 2016, pp. 1–6.
[242] G. Araniti, A. Orsino, L. Militano, L. Wang, A. Iera, Context-Aware Information
Diffusion for Alerting Messages in 5G Mobile Social Networks, IEEE Internet
Things J. 4 (2) (2016) 427–436.
```

```
Computer Networks 193 (2021) 108074
```
[243] C. Suraci, S. Pizzi, A. Iera, G. Araniti, Enhance the Protection of Transmitted
Data in 5G D2D Communications through the Social Internet of Things, in:
Proc. of 29th Annual International Symposium on Personal, Indoor and Mobile
Radio Communications (PIMRC), IEEE, 2018, pp. 376–380.
[244] B. Han, V. Sciancalepore, O. Holland, M. Dohler, H.D. Schotten, D2D-based
Grouped Random Access to Mitigate Mobile Access Congestion in 5G Sensor
Networks, IEEE Commun. Mag. 57 (9) (2019) 93–99.
[245] sony.com, Sony to Release High-Precision GNSS Receiver LSIs for IoT and
Wearable Devices, 2020, [Online] https://www.sony.com/ (Accessed March 3,
2021).
[246] Ó. Belmonte-Fernández, A. Puertas-Cabedo, J. Torres-Sospedra, R. Montoliu-
Colás, S. Trilles-Oliver, An Indoor Positioning System Based on Wearables for
Ambient-Assisted Living, Sensors 17 (1) (2017) 36.
[247] J. Conesa, A. Pérez-Navarro, J. Torres-Sospedra, R. Montoliu, Geographical
and Fingerprinting Data for Positioning and Navigation Systems: Challenges,
Experiences and Technology Roadmap, Academic Press, 2018.
[248] M.A. Al-Ammar, S. Alhadhrami, A. Al-Salman, A. Alarifi, H.S. Al-Khalifa, A.
Alnafessah, M. Alsaleh, Comparative Survey of Indoor Positioning Technolo-
gies, Techniques, and Algorithms, in: Proc. of International Conference on
Cyberworlds, IEEE, 2014, pp. 245–252.
[249] Z. Kasmi, A. Norrdine, J. Blankenbach, Platform Architecture for Decentralized
Positioning Systems, Sensors 17 (5) (2017) 957.
[250] Q. Wang, H. Luo, A. Men, F. Zhao, Y. Huang, An Infrastructure-Free Indoor
Localization Algorithm for Smartphones, Sensors 18 (10) (2018) 3317.
[251] V. Zeimpekis, G.M. Giaglis, G. Lekakos, A Taxonomy of Indoor and Outdoor
Positioning Techniques for Mobile Location Services, ACM SIGecom Exchanges
3 (4) (2002) 19–27.
[252] A.B. Adege, H.-P. Lin, G.B. Tarekegn, Y.Y. Munaye, L. Yen, An Indoor and
Outdoor Positioning using a Hybrid of Support Vector Machine and Deep Neural
Network Algorithms, J. Sens. (2018).
[253] M. Yassin, E. Rachid, A Survey of Positioning Techniques and Location based
Services in Wireless Networks, in: Proc. of IEEE International Conference on
Signal Processing, Informatics, Communication and Energy Systems (SPICES),
IEEE, 2015, pp. 1–5.
[254] A.K. Paul, T. Sato, Localization in Wireless Sensor Networks: A Survey on
Algorithms, Measurement Techniques, Applications and Challenges, J. Sens.
Actuator Netw. 6 (4) (2017) 24.
[255] G.M. Mendoza-Silva, J. Torres-Sospedra, J. Huerta, A Meta-Review of Indoor
Positioning Systems, Sensors 19 (20) (2019) 4507.
[256] P. Pascacio, S. Casteleyn, J. Torres-Sospedra, E.S. Lohan, J. Nurmi, Collaborative
Indoor Positioning Systems: A Systematic Review, Sensors 21 (3) (2021) 1002.
[257] P. Barsocchi, et al., A privacy-by-design architecture for indoor localization
systems, in: Quality of Information and Communications Technology, Springer
International Publishing, Cham, 2020, pp. 358–366.
[258] H. KhademSohi, S. Sharifian, K. Faez, Accuracy-Energy Optimized Location
Estimation Method for Mobile Smartphones by GPS/INS Data Fusion, in: Proc.
of 2nd International Conference of Signal Processing and Intelligent Systems
(ICSPIS), IEEE, 2016, pp. 1–5.
[259] M. Kjaergaard, Location-Based Services on Mobile Phones: Minimizing Power
Consumption, IEEE Pervasive Comput. 11 (1) (2010) 67–73.
[260] A. Ometov, S.V. Bezzateev, J. Kannisto, J. Harju, S. Andreev, Y. Koucheryavy,
Facilitating the Delegation of Use for Private Devices in the Era of the Internet
of Wearable Things, IEEE Internet Things J. 4 (4) (2016) 843–854.
[261] S. He, S.-H.G. Chan, Wi-Fi Fingerprint-based Indoor Positioning: Recent
Advances and Comparisons, IEEE Commun. Surv. Tutor. 18 (1) (2015) 466–490.
[262] D. Vasisht, S. Kumar, D. Katabi, Decimeter-Level Localization with a Single
WiFi Access Point, in: Proc. fo 13th USENIX Symposium on Networked Systems
Design and Implementation, 2016, 165–178.
[263] R. Bharadwaj, C. Parini, A. Alomainy, Experimental Investigation of 3-D Hu-
man Body Localization Using Wearable Ultra-wideband Antennas, IEEE Trans.
Antennas and Propagation 63 (11) (2015) 5035–5044.
[264] T. Otim, L.E. Díez, A. Bahillo, P. Lopez-Iturri, F. Falcone, Effects of the Body
Wearable Sensor Position on the UWB Localization Accuracy, Electronics 8 (11)
(2019) 1351.
[265] D. Dardari, N. Decarli, A. Guerra, F. Guidi, The Future of Ultra-wideband
Localization in RFID, in: Proc. of IEEE International Conference on RFID (RFID),
IEEE, 2016, pp. 1–7.
[266] R. Faragher, R. Harle, Location Fingerprinting with Bluetooth Low Energy
Beacons, IEEE J. Sel. Areas Commun. 33 (11) (2015) 2418–2428.
[267] D. Giovanelli, E. Farella, RSSI or Time-of-Flight for Bluetooth Low Energy Based
Localization? An Experimental Evaluation, in: Proc. of 11th IFIP Wireless and
Mobile Networking Conference (WMNC), IEEE, 2018, pp. 1–8.
[268] A.K. Ng, L.K. Chan, H.Y. Lau, A Low-Cost Lighthouse-Based Virtual Reality Head
Tracking System, in: Proc. of International Conference on 3D Immersion (IC3D),
IEEE, 2017, pp. 1–5.
[269] S. Shao, A. Khreishah, J. Paez, PassiveRETRO: Enabling Completely Passive
Visible Light Localization for IoT Applications, in: Proc. of IEEE Conference on
Computer Communications (INFOCOM), IEEE, 2019, pp. 1540–1548.
[270] Z. Wang, Z. Yang, Q. Huang, L. Yang, Q. Zhang, ALS-P: Light Weight Visible
Light Positioning via Ambient Light Sensor, in: Proc. of IEEE Conference on
Computer Communications (INFOCOM), IEEE, 2019, pp. 1306–1314.

```
[271] B.C. Fargas, M.N. Petersen, GPS-Free Geolocation Using LoRa in Low-Power
WANs, in: Proc. of Global Internet of Things Summit (GIoTS), IEEE, 2017, pp.
1–6.
[272] A. Mackey, P. Spachos, LoRa-Based Localization System for Emergency Ser-
vices in GPS-Less Environments, in: Proc. of IEEE Conference on Computer
Communications Workshops (INFOCOM WKSHPS), IEEE, 2019, pp. 939–944.
[273] C. Duan, L. Yang, Q. Lin, Y. Liu, Tagspin: High Accuracy Spatial Calibration of
RFID Antennas via Spinning Tags, IEEE Trans. Mob. Comput. 17 (10) (2018)
2438–2451.
[274] F. Xiao, Z. Wang, N. Ye, R. Wang, X.-Y. Li, One More Tag Enables Fine-
Grained RFID Localization and Tracking, IEEE/ACM Trans. Netw. 26 (1) (2017)
161–174.
[275] Y. Zhao, Y. Liu, L.M. Ni, VIRE: Active RFID-Based Localization Using Vir-
tual Reference Elimination, in: Proc. of International Conference on Parallel
Processing (ICPP), IEEE, 2007, p. 56.
[276] Y.-L. Chen, D. Liu, S. Wang, Y.-F. Li, X.-S. Zhang, Self-powered smart active
RFID tag integrated with wearable hybrid nanogenerator, Nano Energy 64
(2019) 103911.
[277] A. Bröring, S. Schmid, C.-K. Schindhelm, A. Khelil, S. Käbisch, D. Kramer, D.
Le Phuoc, J. Mitic, D. Anicic, E. Teniente, Enabling IoT Ecosystems through
Platform Interoperability, IEEE software 34 (1) (2017) 54–61.
[278] N. Pathak, A. Mukherjee, S. Misra, Reconfigure and Reuse: Interoperable
Wearables for Healthcare IoT, in: Proc. of IEEE Conference on Computer
Communications, IEEE, 2020, pp. 20–29.
[279] M. Noura, M. Atiquzzaman, M. Gaedke, Interoperability in Internet of Things:
Taxonomies and Open Challenges, Mob. Netw. Appl. 24 (3) (2019) 796–809.
[280] O. Bello, S. Zeadally, M. Badra, Network Layer Inter-Operation of Device-to-
Device Communication technologies in Internet of Things (IoT), Ad Hoc Netw.
57 (2017) 52–62.
[281] S.D. Nagowah, H.B. Sta, B. Gobin-Rahimbux, An Overview of Semantic Inter-
operability Ontologies and Frameworks for IoT, in: Proc. of 6th International
Conference on Enterprise Systems (ES), IEEE, 2018, pp. 82–89.
[282] P. Murdock, L. Bassbouss, M. Bauer, M.B. Alaya, R. Bhowmik, P. Brett, R.N.
Chakraborty, M. Dadas, J. Davies, W. Diab, et al., Semantic interoperability for
the Web of Things, Médiathèque Télécom Sudparis & Institut Mines-Télécom
Business School, 2016, [Online] (Accessed March 3, 2021) https://tel.archives-
ouvertes.fr/UNIV-PARIS-SACLAY/hal-01362033v1.
[283] O. Vermesan, Advancing IoT Platforms Interoperability, Gistrup: River
Publishers, 2018.
[284] N.-G. Wunsch, LexisNexis PatentSight, Largest Wearables Patent Owners
Worldwide from 2010 to 2019, Statista.
[285] J.E. Mück, B. Ünal, H. Butt, A.K. Yetisen, Market and Patent Analyses of
Wearables in Medicine, Trends Biotechnol. 37 (6) (2019) 563–566.
[286] S. Osman, R. Marks, Methods for Optimizing Positioning of Content on a Screen
of a Head Mounted Display, 2019.
[287] T. Tamai, T. Oya, Information Processing Device, Information Processing
Method, Information Processing Program, and Recording Medium, 2018.
[288] C. Russey, RealWear Raises $80 million for Augmented Reality Headset for Con-
nected Workers, Wearabe Technologies Show Medica [Online] (Accessed March
3, 2021), 2019, https://www.wearable-technologies.com/2019/07/realwear-
raises-80-million-for-augmented-reality-headset-for-connected-workers/.
[289] S. Draper, Kopin Unveils World’s First Voice-Controlled AR Headset,
Wearabe Technologies Show Medica [Online] (accessed march 3, 2021),
2018, https://www.wearable-technologies.com/2018/06/kopin-unveils-worlds-
first-voice-controlled-ar-headset/.
[290] S. Draper, HMDmd-Kopin Partnership to Develop Next Gen Wearable Displays
for MedTech, Wearabe Technologies Show Medica [Online] (accessed march 3,
2021), 2019, https://www.wearable-technologies.com/2019/06/hmdmd-kopin-
partnership-to-develop-next-gen-wearable-displays-for-medtech/.
[291] B. Heater, Microsoft and Trimble Made a Hard Hat with HoloLens Built-in,
2019, [Online] (Accessed March 3, 2021) https://techcrunch.com/2019/02/24/
microsoft-and-trimble-made-a-hardhat-with-hololens-built-in/.
[292] Zebra Technologies Corp. Zebra’S Total Wearable Solutions: Double-digit
Productivity Gains over Prior Generation Zebra Wearable Devices, 2019,
[Online] (Accessed March 3, 2021) https://www.zebra.com/us/en/products/
mobile-computers/wearable-computers.html.
[293] R. Socher, Vuzix Partners With Plessey to Develop Next-Gen AR
Smartglasses Using MicroLED Technology, Wearabe Technologies Show
Medica [Online] (accessed march 3, 2021), 2018, https://www.wearable-
technologies.com/2018/06/vuzix-partners-with-plessey-to-develop-next-gen-
ar-smartglasses-using-microled-technology/.
[294] C. Russey, Tesla Files Patent for Google Glass-Like AR System for
Faster, Accurate Vehicle Production, 2018, [Online] (Accessed March 3,
2021) https://www.wearable-technologies.com/2018/12/tesla-files-patent-for-
google-glass-like-ar-system-for-faster-accurate-vehicle-production/.
[295] Bose Corporation, Bose Frames Rondo: Audio Sunglasses, 2019, [Online]
(Accessed March 3, 2021) https://www.bose.com/en_us/products/frames/bose-
frames-rondo.html.
[296] M. Sawh, Nreal Light Smartglasses Provide Hope Mixed Reality for the Masses
Will Be Here Soon, 2019, [Online] (Accessed March 3, 2021) https://www.
wareable.com/ar/nreal-mixed-reality-glasses-review-7018.
```

```
Computer Networks 193 (2021) 108074
```
[297] S. Mashal, G. Hoelzl, M. Kranz, Valkyrie Project: Flying Immersion in Virtual
Reality, in: Proc. of 11th International Conference on Virtual Worlds and Games
for Serious Applications (VS-Games), IEEE, 2019, pp. 1–4.
[298] C. Russey, This Smart Vest Aims to Predict Your Heart-Attack Before it
Happens, Wearabe Technologies Show Medica [Online] (accessed march 3,
2021), 2019, https://www.wearable-technologies.com/2019/01/ces-2019-this-
smart-vest-aims-to-predict-your-heart-attack-before-it-happens/.
[299] K. Matthews, Upright Vs. Lumo Lift: Which Posture Gadget Gets the Best
Reviews?, 2017, [Online] (Accessed March 3, 2021) https://geardiary.com/
2017/11/18/upright-vs-lumo-lift-posture-gadget-gets-best-reviews/.
[300] J. Stables, Best Heart Rate Monitor 2019: HRM Watches and Chest Straps
Compared, 2019, [Online] (Accessed March 3, 2021) https://www.wareable.
com/fitness-trackers/best-heart-rate-monitor-and-watches.
[301] J. Su, Apple Watch 4 Is Now An FDA Class 2 Medical Device: Detects
Falls, Irregular Heart Rhythm, 2018, [Online] (Accessed March 3,
2021) https://www.forbes.com/sites/jeanbaptiste/2018/09/14/apple-
watch-4-is-now-an-fda-class-2-medical-device-detects-falls-irregular-heart-
rhythm/#113ff69a2071.
[302] S. Draper, FDA Approves First Cochlear Implants for Single-Sided Deaf-
ness and Asymmetric Hearing Loss, 2019, [Online] (Accessed March
3, 2021) https://www.wearable-technologies.com/2019/07/fda-approves-first-
cochlear-implants-for-single-sided-deafness-and-asymmetric-hearing-loss/.
[303] W.W. Lee, Y.J. Tan, H. Yao, S. Li, H.H. See, M. Hon, K.A. Ng, B. Xiong, J.S.
Ho, B.C. Tee, A Neuro-Inspired Artificial Peripheral Nervous System for Scalable
Electronic Skins, Sci. Robot. 4 (32) (2019) eaax2198.
[304] M.-K. Schöppl, EVER Pharma Launches Innovative, Patient Friendly Subcuta-
neous Pump for Parkinson’s Disease, 2019, BusinessWire [Online] (Accessed
March 3, 2021) https://www.businesswire.com/news/home/20190630005001/
en/Pharma-Launches-Innovative-Patient-Friendly-Subcutaneous-Pump.
[305] A. Gruentzig, Wearable Device: WO2015183470, 2017.
[306] D.M. Kirsch, B. Chen, H. Vashi, System and Method for Vehicle Control
Integrating Health Priority Alerts of Vehicle Occupants: US20160297359A1,
2016.
[307] D. Lumb, We Need Sony’s Wearable Air Conditioner Right Now, Techradar
[Online] (Accessed March 3, 2021), 2019, https://www.techradar.com/news/
we-need-sonys-wearable-air-conditioner-right-now.
[308] Embr Labs, Your Personal Thermostat, 2020, [Online] (Accessed March 3, 2021)
https://embrlabs.com.
[309] IMeasureU, The Best Wearable Technology for Athletes, 2019, [Online]
(Accessed March 3, 2021) https://imeasureu.com/2019/08/29/best-wearable-
technology-athletes/.
[310] Catapult, Wearable Technology. Products, 2020, [Online] (Accessed March 3,
2021) https://www.catapultsports.com/products.
[311] STATSports, STATSports Products, 2020, [Online] (Accessed March 3, 2021)
https://statsports.com/products/.
[312] P.R. Bailey, Wearable Device for Fishing: US20150057968A1, 2019.
[313] Xsens, 2020, [Online] (Accessed March 3, 2021) https://www.xsens.com/.
[314] Allied Business Intelligence, Inc, in: In-Vehicle Wearable Integration, Tech. Rep.
Technical Report, 2014.
[315] K. Roberts, SMK Electronics and CAARESYS Partner to Develop Biometric
Passenger Monitoring Technology, BusinessWire, 2019, [Online] (Accessed
March 3, 2021) https://www.zepp.com/en-us/golf/smart-coach/.
[316] S. Vhaduri, C. Poellabauer, Biometric-based Wearable User Authentication
During Sedentary and Non-Sedentary Periods, arXiv preprint arXiv:1811.07060.
[317] Y. Chen, G.A. Yuval, M.J. Sinclair, Mobile Device Security Using Wearable
Security Tokens, 2015, uS Patent 9, 135, 620.
[318] X. Huang, Z. Nie, H. Yi, Wearable Security Device, 2017, uS Patent App.
15/229, 393.
[319] D.M. Lerner, User-Wearable Secured Devices Provided Assuring Authentication
and Validation of Data Storage and Transmission, 2018, uS Patent 10, 154,
031.
[320] N. Tanaka, V. Elgort, J. Danielson, A. Kalachev, J. Wong, U.R. Bhat, L. Copere,
M. Kataoka, et al., Smart Wearable Devices and Methods for Acquisition of
Sensorial Information from Wearable Devices to Activate Functions in Other
Devices, 2017, uS Patent App. 15/229, 393.
[321] A. Parara, S. Sekka, Wearable Care Security Smart Watch Device, 2016, uS
Patent App. 15/162, 121.
[322] B. Murison, Remote Drive and Wearable Adult Devices, 2018, uS Patent App.
15/764, 201.
[323] F. Sedic, Wearable Massager for Couples, 2016, uS Patent 9, 474, 681.
[324] A. Scheuring, A. Guldahl, L.I. Andersen, K.R. Ellekrans, Devices and Methods
for Sexual Wellness, 2018, uS Patent 10, 022, 293.
[325] Wearable Electroactive Fabrics Integrated in Garments, 2021, [Online] https:
//cordis.europa.eu/project/id/825232 (Accessed March 3, 2021).
[326] Smart and Flexible Energy Supply Platform for Wearable Electronics, 2021,
[Online] https://cordis.europa.eu/project/rcn/219473/factsheet/en (Accessed
March 3, 2021).
[327] Personalised Body Sensor Networks with Built-In Intelligence for Real-Time
Risk Assessment and Coaching of Ageing workers, in All Types of Working
and Living Environments, 2021, [Online] https://cordis.europa.eu/project/id/
826304 (Accessed March 3, 2021).

```
[328] RAIS: Real-time Analytics for the Internet of Sports, 2021, [Online] https:
//cordis.europa.eu/project/id/813162 (Accessed March 3, 2021).
[329] Exceptional Sense of Touch for Robots and Prosthetics, 2021, [On-
line] http://news.nus.edu.sg/research/exceptional-touch-robots-prosthetics (Ac-
cessed March 3, 2021).
[330] S. Lee, D. Sasaki, D. Kim, M. Mori, T. Yokota, H. Lee, S. Park, K. Fukuda,
M. Sekino, K. Matsuura, et al., Ultrasoft Electronics to Monitor Dynamically
Pulsing Cardiomyocytes, Nature Nanotechnol. 14 (2) (2019) 156–160.
[331] Don’t Go Breaking My Heart, 2021, [Online] https://www.u-tokyo.ac.jp/focus/
en/press/z0508_00021.html (Accessed March 3, 2021).
[332] B. Zhang, D.K. Sodickson, M.A. Cloos, A High-Impedance Detector-Array Glove
for Magnetic Resonance Imaging of the Hand, Nat. Biomed. Eng. 2 (8) (2018)
570–577.
[333] A.J. Bandodkar, P. Gutruf, J. Choi, K. Lee, Y. Sekine, J.T. Reeder, W.J.
Jeang, A.J. Aranyosi, S.P. Lee, J.B. Model, et al., Battery-Free, Skin-Interfaced
Microfluidic/Electronic Systems for Simultaneous Electrochemical, Colorimetric,
and Volumetric Analysis of Sweat, Sci. Adv. 5 (1) (2019) eaav3294.
[334] Blood and Sweat Take Training App to the Next Level, 2021, [Online]
https://www.kth.se/en/aktuellt/nyheter/blod-och-svett-tar-traningsappen-till-
nasta-niva-1.901859 (Accessed March 3, 2021).
[335] H. Garcia-Molina, M. Joglekar, A. Marcus, A. Parameswaran, V. Verroios,
Challenges in Data Crowdsourcing, IEEE Trans. Knowl. Data Eng. 28 (4) (2016)
901–911.
[336] M. Al-Soh, I.A. Zualkernan, An MQTT-based Context-Aware Wearable Assess-
ment Platform for Smart Watches, in: Proc. of 17th International Conference
on Advanced Learning Technologies (ICALT), IEEE, 2017, pp. 98–100.
[337] W. Feng, Z. Yan, H. Zhang, K. Zeng, Y. Xiao, Y.T. Hou, A.Survey.on. Security,
Privacy, A Survey on Security Privacy and Trust in Mobile Crowdsourcing, IEEE
Internet Things J. 5 (4) (2017) 2971–2992.
[338] D. Ravi, C. Wong, B. Lo, G.-Z. Yang, A Deep Learning Approach to On-Node
Sensor Data Analytics for Mobile or Wearable Devices, IEEE J. Biomed. Health
Inf. 21 (1) (2016) 56–64.
[339] A. Harris, H. True, Z. Hu, J. Cho, N. Fell, M. Sartipi, Fall Recognition
Using Wearable Technologies and Machine Learning Algorithms, in: Proc. of
International Conference on Big Data (Big Data), IEEE, 2016, pp. 3974–3976.
[340] J. Ker, L. Wang, J. Rao, T. Lim, Deep Learning Applications in Medical Image
Analysis, IEEE Access 6 (2017) 9375–9389.
[341] O.D. Lara, M.A. Labrador, A Survey on Human Activity Recognition Using
Wearable Sensors, IEEE Commun. Surv. Tutor. 15 (3) (2012) 1192–1209.
[342] Q. Zhu, Z. Chen, Y.C. Soh, A Novel Semisupervised Deep Learning Method for
Human Activity Recognition, IEEE Trans. Ind. Inf. 15 (7) (2018) 3821–3830.
[343] Y. Ma, H. Ghasemzadeh, LabelForest: Non-Parametric Semi-Supervised Learning
for Activity Recognition, in: Proc. of AAAI Conference on Artificial Intelligence,
33, 2019, 4520–4527.
[344] M. Lv, L. Chen, T. Chen, G. Chen, Bi-View Semi-Supervised Learning Based
Semantic Human Activity Recognition Using Accelerometers, IEEE Trans. Mob.
Comput. 17 (9) (2018) 1991–2001.
[345] Q.W. Oung, M. Hariharan, H.L. Lee, S.N. Basah, M. Sarillee, C.H. Lee, Wearable
Multimodal Sensors for Evaluation of Patients with Parkinson Disease, in:
Proc. of IEEE International Conference on Control System, Computing and
Engineering (ICCSCE), IEEE, 2015, pp. 269–274.
[346] N. Lu, H. Jeong, Wireless Electronic Tattoos, Proc. of Structural Health
Monitoring..
[347] S. Geisler, Body Art Gets Smart, Cell 174 (6) (2018) 1331.
[348] A. Tastanova, M. Folcher, M. Müller, G. Came-nisch, A. Ponti, T. Horn, M.S.
Tikhomirova, M. Fus-senegger, Synthetic Biology-Based Cellular Biomedical
Tattoo for Detection of Hypercalcemia Associated with Cancer, Sci. Transl. Med.
10 (437) (2018) 8562.
[349] K.Y. Goud, C. Moonla, R.K. Mishra, C. Yu, R. Narayan, I. Litvan, J. Wang,
Wearable Electrochemical Microneedle Sensor for Continuous Monitoring of
Levodopa: Toward Parkinson Management, ACS Sens. 4 (8) (2019) 2196–2204.
[350] K. Kaewkannate, S. Kim, A Comparison of Wearable Fitness Devices, BMC Public
Health 16 (1) (2016) 433.
[351] L. Klus, E.S. Lohan, C. Granell, J. Nurmi, Crowdsourcing Solutions for Data
Gathering from Wearables, in: Proc. of XXXV Finnish URSI Convention on Radio
Science, 2019.
[352] D.R. Witt, R.A. Kellogg, M.P. Snyder, J. Dunn, Windows Into Human Health
Through Wearables Data Analytics, Curr. Opinion Biomed. Eng. 9 (2019) 28–46.
[353] B.R. Bloem, E.J. Henderson, E.R. Dorsey, M.S. Okun, N. Okubadejo, P. Chan,
J. Andrejack, S.K. Darweesh, M. Munneke, Integrated and Patient-centred
Management of Parkinson’s Disease: A Network Model for Reshaping Chronic
Neurological Care, The Lancet Neurology.
[354] P. Stanley-Marbell, A. Alaghi, M. Carbin, E. Darulova, L. Dolecek, A. Gerstlauer,
G. Gillani, D. Jevdjic, T. Moreau, A. Daglis, et al., Exploiting Errors for
Efficiency: A Survey from Circuits to Algorithms, ACM Comput. Surv. (CSUR)
53 3:51.
[355] G. Wilson, J. Bryan, K. Cranston, J. Kitzes, L. Nederbragt, T.K. Teal, Good
Enough Practices in Scientific Computing, PLoS Comput. Biol. 13 (6) (2017)
e1005510.
[356] Q. Xu, T. Mytkowicz, N.S. Kim, Approximate Computing: A Survey, IEEE Des.
Test 33 (1) (2015) 8–22.
```

```
Computer Networks 193 (2021) 108074
```
[357] S. Mittal, A Survey of Techniques for Approximate Computing, ACM Comput.
Surv. 48 (4) (2016) 1–33.
[358] N.T. Ti, L.B. Le, Computation Offloading Leveraging Computing Resources from
Edge Cloud and Mobile Peers, in: Proc. of IEEE International Conference on
Communications (ICC), IEEE, 2017, pp. 1–6.
[359] F. Jalali, O.J. Smith, T. Lynar, F. Suits, Cognitive IoT Gateways: Automatic Task
Sharing and Switching Between Cloud and Edge/Fog Computing, in: Proc. of
the SIGCOMM Posters and Demos, 2017, 121–123.
[360] F. Jalali, T. Lynar, O.J. Smith, R.R. Kolluri, C.V. Hardgrove, N. Waywood, F.
Suits, Dynamic Edge Fabric Environment: Seamless and Automatic Switching
among Resources at the Edge of IoT Network and Cloud, in: Proc. of IEEE
International Conference on Edge Computing (EDGE), IEEE, 2019, pp. 77–86.
[361] A. Das, A. Leaf, C.A. Varela, S. Patterson, Skedulix: Hybrid Cloud Scheduling
for Cost-Efficient Execution of Serverless Applications, arXiv preprint arXiv:
2006.03720.
[362] O. Chukhno, N. Chukhno, G. Araniti, C. Campolo, A. Iera, A. Molinaro, Optimal
Placement of Social Digital Twins in Edge IoT Networks, Sensors 20 (21) (2020)
6181.
[363] C. Campolo, A. Iera, A. Molinaro, G. Ruggeri, MEC Support for 5G-V2X Use
Cases through Docker Containers, in: Proc. of IEEE Wireless Communications
and Networking Conference (WCNC), IEEE, 2019, pp. 1–6.
[364] Q. Fan, N. Ansari, On Cost Aware Cloudlet Placement for Mobile Edge
Computing, IEEE/CAA J. Autom. Sinica 6 (4) (2019) 926–937.
[365] S. Wang, J. Xu, N. Zhang, Y. Liu, A Survey on Service Migration in Mobile
Edge Computing, IEEE Access 6 (2018) 23511–23528.
[366] X. Yu, M. Guan, M. Liao, X. Fan, Pre-Migration of Vehicle to Network Services
Based on Priority in Mobile Edge Computing, IEEE Access 7 (2018) 3722–3730.
[367] L. Wang, L. Jiao, J. Li, J. Gedeon, M. Mühlhäuser, MOERA: Mobility-agnostic
Online Resource Allocation for Edge Computing, IEEE Trans. Mob. Comput. 18
(8) (2018) 1843–1856.
[368] S. Wang, R. Urgaonkar, M. Zafer, T. He, K. Chan, K.K. Leung, Dynamic
Service Migration in Mobile Edge Computing Based on Markov Secision Process,
IEEE/ACM Trans. Netw. 27 (3) (2019) 1272–1288.
[369] S. Padalkar, A. Korlekar, U. Pacharaney, Data Gathering in Wireless Sensor
Network for Energy Efficiency with and without Compressive Sensing at Sensor
Node, in: Proc. of International Conference on Communication and Signal
Processing (ICCSP), IEEE, 2016, pp. 1356–1359.
[370] A. Fragkiadakis, P. Charalampidis, E. Tragos, Adaptive Compressive Sensing for
Energy Efficient Smart Objects in IoT Applications, in: Proc. of 4th International
Conference on Wireless Communications, Vehicular Technology, Information
Theory and Aerospace & Electronic Systems (VITAE), IEEE, 2014, pp. 1–5.
[371] M. Liyanage, I. Ahmad, A.B. Abro, A. Gurtov, M. Ylianttila, A Comprehensive
Guide To 5G Security, John Wiley & Sons, 2018.
[372] P. Datta, A.S. Namin, M. Chatterjee, A Survey of Privacy Concerns in Wearable
Devices, in: 2018 IEEE International Conference on Big Data (Big Data), IEEE,
2018, pp. 4549–4553.
[373] E. Huang, J.-P. Onnela, Activity Classification Using Smartphone Gyroscope and
Accelerometer Data, arXiv preprint arXiv:1903.12616.
[374] L. Simpson, M.M. Maharaj, R.J. Mobbs, The Role of Wearables in Spinal Posture
Analysis: A Systematic Review, BMC Musculoskelet. Disorders 20 (1) (2019) 55.
[375] A.M. Sabatini, V. Genovese, A Sensor Fusion Method for Tracking Vertical
Velocity and Height Based on Inertial and Barometric Altimeter Measurements,
Sensors 14 (8) (2014) 13324–13347.
[376] L. Ozella, L. Gauvin, L. Carenzo, M. Quaggiotto, P.L. Ingrassia, M. Tizzoni,
A. Panisson, D. Colombo, A. Sapienza, K. Kalimeri, et al., Wearable Proximity
Sensors for Monitoring a Mass Casualty Incident Exercise: Feasibility Study, J.
Med. Internet Res. 21 (4) (2019) e12251.
[377] S. Bian, B. Zhou, H. Bello, P. Lukowicz, A Wearable Magnetic Field Based
Proximity Sensing System for Monitoring COVID-19 Social Distancing, in: Proc.
of International Symposium on Wearable Computers, 2020, 22–26.
[378] J. Martín-Vaquero, A. Hernández Encinas, A. Queiruga-Dios, J. José Bullón,
A. Martínez-Nova, J. Torreblanca González, C. Bullón-Carbajo, Review on
Wearables to Monitor Foot Temperature in Diabetic Patients, Sensors 19 (4)
(2019) 776.
[379] H. Han, H. Jang, S.W. Yoon, Novel Wearable Monitoring System of Forward
Head Posture Assisted by Magnet-Magnetometer Pair and Machine Learning,
IEEE Sens. J., 2019.
[380] W. Zhuang, Y. Chen, J. Su, B. Wang, C. Gao, Design of human activity
recognition algorithms based on a single wearable IMU sensor, Int. J. Sens.
Netw. 30 (3) (2019) 193–206.
[381] A. Mihoub, G. Lefebvre, Wearables and Social Signal Processing for Smarter
Public Presentations, ACM Trans. Interactive Intell. Syst. (TiiS) 9 (2–3) (2019)
1–24.
[382] V. Dissanayake, D.S. Elvitigala, H. Zhang, C. Weerasinghe, S. Nanayakkara,
CompRate: Power Efficient Heart Rate and Heart Rate Variability Monitoring on
Smart Wearables, in: Proc. of 25th ACM Symposium on Virtual Reality Software
and Technology, 2019, 1–8.
[383] C.L. Karmen, M.A. Reisfeld, M.K. McIntyre, R. Timmermans, W. Frishman, The
Clinical Value of Heart Rate Monitoring Using an Apple Watch, Cardiol. Rev.
27 (2) (2019) 60–62.

```
[384] O. Badreddin, R. Castillo, L. Lessard, M. Albanese, Towards Improved Per-
formance and Compliance in Healthcare Using Wearables and Bluetooth
Technologies, in: Proc. of 25th Annual International Conference on Computer
Science and Software Engineering, 2015, 239–242.
[385] D.R. Seshadri, R.T. Li, J.E. Voos, J.R. Rowbottom, C.M. Alfes, C.A. Zorman, C.K.
Drummond, Wearable Sensors for Monitoring the Physiological and Biochemical
Profile of the Athlete, NPJ Digital Med. 2 (1) (2019) 1–16.
[386] M. D’Arco, A. Renga, A. Ceccarelli, F. Brancati, A. Bondavalli, Enhancing
Workers Safety in Worksites through Augmented GNSS Sensors, Measurement
117 (2018) 144–152.
[387] L. Guanke, Y. Jianan, Y. Wen, Z. Yanling, Research on Seamless Positioning
of Power Wearables Based on GPS/UWB Combination, in: Proc. of IEEE Inter-
national Conference on Computer and Communication Engineering Technology
(CCET), IEEE, 2018, pp. 123–127.
[388] H. Yoon, S.-H. Park, K.-T. Lee, Exploiting Ambient Light Sensor for Authen-
tication on Wearable Devices, in: Proc. of 4th International Conference on
Cyber Security, Cyber Warfare, and Digital Forensic (CyberSec), IEEE, 2015,
pp. 95–100.
[389] S.K. Polu, S. Polu, NFC Based Smart Healthcare Services System, Int. J. Innov.
Res. Sci. Technol. 5 (7) (2018) 45–48.
[390] C. Hill, Wearables–The Future of Biometric Technology? Biometric Technol.
Today 2015 (8) (2015) 5–9.
[391] H. Sellahewa, N. Ibrahim, S. Zeadally, Biometric Authentication for Wearables,
in: Biometric-Based Physical and Cybersecurity Systems, Springer, 2019, pp.
355–386.
[392] M. Nguyen, M.O. Gani, V. Raychoudhury, Yours Truly? Survey on Accessibility
of Our Personal Data in the Connected World, in: Proc. of IEEE International
Conference on Pervasive Computing and Communications Workshops (PerCom
Workshops), IEEE, 2019, pp. 292–297.
[393] A. Ometov, P. Masek, L. Malina, R. Florea, J. Hosek, S. Andreev, J. Hajny,
J. Niutanen, Y. Koucheryavy, Feasibility Characterization of Cryptographic
Primitives for Constrained (Wearable) IoT Devices, in: Proc. of International
Conference on Pervasive Computing and Communication Workshops (PerCom
Workshops), IEEE, 2016, pp. 1–6.
[394] M. Wang, Z. Yan, A Survey on Security in D2D Communications, Mob. Netw.
Appl. 22 (2) (2017) 195–208.
[395] R.I. Ansari, C. Chrysostomou, S.A. Hassan, M. Guizani, S. Mumtaz, J. Rodriguez,
J.J. Rodrigues, 5G D2D networks: Techniques, Challenges, and Future Prospects,
IEEE Syst. J. 12 (4) (2017) 3970–3984.
[396] S.R. Jondhale, M. Sharma, R. Maheswar, R. Shubair, A. Shelke, Comparison of
Neural Network Training Functions for RSSI Based Indoor Localization Problem
in WSN, in: Handbook of Wireless Sensor Networks: Issues and Challenges in
Current Scenario’s, Springer, 2020, pp. 112–133.
[397] X.B. Maxama, E.D. Markus, A Survey on Propagation Challenges in Wireless
Communication Networks over Irregular Terrains, in: Proc. of Open Innovations
Conference (OI), IEEE, 2018, pp. 79–86.
[398] K. Yu, K. Wen, Y. Li, S. Zhang, K. Zhang, A Novel NLOS Mitigation Algorithm
for UWB Localization in Harsh Indoor Environments, IEEE Trans. Veh. Technol.
68 (1) (2018) 686–699.
[399] W. Wei, X. Jin-Yu, Z. Zhong-Liang, A New NLOS Error Mitigation Algorithm in
Location Estimation, IEEE Trans. Veh. Technol. 54 (6) (2005) 2048–2053.
[400] H. Miao, K. Yu, M.J. Juntti, Positioning for NLOS propagation: Algorithm
derivations and Cramer–Rao Bounds, IEEE Trans. Veh. Technol. 56 (5) (2007)
2568–2580.
[401] R.M. Vaghefi, R.M. Buehrer, Cooperative Localization in NLOS Environ-
ments Using Semidefinite Programming, IEEE Commun. Lett. 19 (8) (2015)
1382–1385.
[402] V. Shubina, A. Ometov, S. Andreev, D. Niculescu, E.S. Lohan, Privacy Versus Lo-
cation Accuracy in Opportunistic Wearable Networks, in: Proc. of International
Conference on Localization and GNSS (ICL-GNSS), IEEE, 2020, pp. 1–6.
[403] F. Potortì, A. Crivello, P. Barsocchi, F. Palumbo, Evaluation of Indoor Lo-
calisation Systems: Comments on the ISO/IEC 18305 Standard, in: Proc. of
International Conference on Indoor Positioning and Indoor Navigation (IPIN),
2018, 1–7.
[404] ISO, Information Technology – Real Time Localization System – Test and
Evaluation of Localization and Tracking Systems, Standard, International
Organization for Standardization, Geneva, CH, 2016.
[405] F. Furfari, A. Crivello, P. Barsocchi, F. Palumbo, F. Potortí, What is next for
Indoor Localisation? Taxonomy, Protocols, and Patterns for Advanced Location
Based Services, in: Proc. of International Conference on Indoor Positioning and
Indoor Navigation (IPIN), 2019, 1–8.
[406] A. Ometov, P. Masek, J. Urama, J. Hosek, S. Andreev, Y. Koucheryavy,
Implementing Secure Network-Assisted D2D Framework in Live 3GPP LTE
Deployment, in: Proc. of IEEE International Conference on Communications
Workshops (ICC), IEEE, 2016, pp. 749–754.
[407] K. Wang, J. Alonso-Zarate, M. Dohler, Energy-Efficiency of LTE for Small
Data Machine-to-Machine Communications, in: Proc. of IEEE International
Conference on Communications (ICC), IEEE, 2013, pp. 4120–4124.
[408] G. Rigazzi, N.K. Pratas, P. Popovski, R. Fantacci, Aggregation and Trunking of
M2M Traffic via D2D Connections, in: Proc. of IEEE International Conference
on Communications (ICC), IEEE, 2015, pp. 2973–2978.
```

```
Computer Networks 193 (2021) 108074
```
[409] Z. Zhang, C. Wang, H. Yu, M. Wang, S. Sun, Power Optimization Assisted
Interference Management for D2D Communications in mmWave Networks, IEEE
Access 6 (2018) 50674–50682.
[410] A. Gupta, R.K. Jha, A Survey of 5G Network: Architecture and Emerging
Technologies, IEEE Access 3 (2015) 1206–1232.
[411] Y. He, J. Ren, G. Yu, Y. Cai, D2D Communications Meet Mobile Edge Computing
for Enhanced Computation Capacity in Cellular Networks, IEEE Trans. Wireless
Commun. 18 (3) (2019) 1750–1763.
[412] G. Araniti, A. Orsino, L. Militano, G. Putrino, S. Andreev, Y. Koucheryavy, A.
Iera, Novel D2D-based relaying method for multicast services over 3GPP LTE-A
systems, in: Proc. of IEEE International Symposium on Broadband Multimedia
Systems and Broadcasting (BMSB), IEEE, 2017, pp. 1–5.
[413] L. Militano, M. Condoluci, G. Araniti, A. Molinaro, A. Iera, G.-M. Muntean,
Single Frequency-based Device-to-Device-enhanced Video Delivery for Evolved
Multimedia Broadcast and Multicast Services, IEEE Trans. Broadcast. 61 (2)
(2015) 263–278.
[414] M. Kritzler, M. Bäckman, A. Tenfält, F. Michahelles, Wearable Technology as
a Solution for Workplace Safety, in: Proc. of 14th International Conference on
Mobile and Ubiquitous Multimedia, 2015, 213–217.
[415] E. Svertoka, A. Rusu-Casandra, I. Marghescu, State-of-the-Art of Industrial
Wearables: A Systematic Review, in: Proc. of 13th International Conference
on Communications (COMM), IEEE, 2020, pp. 411–415.
[416] S. Kim, Y. Sharif, I. Nasim, Human Electromagnetic Field Exposure in Wearable
Communications: A Review, arXiv preprint arXiv:1912.05282.
[417] I. Nasim, S. Kim, Human EMF Exposure in Wearable Networks for Internet
of Battlefield Things, in: Proc. of IEEE Military Communications Conference
(MILCOM), IEEE, 2019, pp. 1–6.
[418] G. Kiruthiga, A. Sharmila, P. Mahalakshmi, M. Muruganandam, Power Optimi-
sation for Wearable Heart Rate Measurement Device with Wireless Charging,
J. Med. Eng. Technol. 41 (4) (2017) 288–297.
[419] M.A. Razzaque, S. Dobson, Energy-Efficient Sensing in Wireless Sensor Networks
Using Compressed Sensing, Sensors 14 (2) (2014) 2822–2859.
[420] Y. Zhang, Y. Zhao, J. Ren, W. Weng, H. Peng, Advances in Wearable
Fiber-Shaped Lithium-Ion Batteries, Adv. Mater. 28 (22) (2016) 4524–4531.
[421] M. Magno, D. Boyle, Wearable Energy Harvesting: From Body to Battery, in:
Proc. of 12th International Conference on Design & Technology of Integrated
Systems in Nanoscale Era (DTIS), IEEE, 2017, pp. 1–6.
[422] M. Magno, D. Kneubühler, P. Mayer, L. Benini, Micro Kinetic Energy Harvesting
for Autonomous Wearable Devices, in: Proc. of International Symposium on
Power Electronics, Electrical Drives, Automation and Motion (SPEEDAM), IEEE,
2018, pp. 105–110.
[423] P. Jokic, M. Magno, Powering Smart Wearable Systems with Flexible Solar
Energy Harvesting, in: Proc. of International Symposium on Circuits and
Systems (ISCAS), IEEE, 2017, pp. 1–4.
[424] L.V. Thekkekara, M. Gu, Large-Scale Waterproof and Stretchable Textile-
Integrated Laser-Printed Graphene Energy Storages, Sci. Rep. 9 (1) (2019)
1–7.
[425] K.N. Bocan, E. Sejdić, Adaptive Transcutaneous Power Transfer to Implantable
Devices: A State of the Art Review, Sensors 16 (3) (2016) 393.
[426] K. Agarwal, R. Jegadeesan, Y.-X. Guo, N.V. Thakor, Wireless Power Transfer
Strategies for Implantable Bioelectronics, IEEE Rev. Biomed. Eng. 10 (2017)
136–161.
[427] T. Ghomian, S. Mehraeen, Survey of Energy Scavenging for Wearable and
Implantable Devices, Energy 178 (2019) 33–49.
[428] J. Portilla, G. Mujica, J.-S. Lee, T. Riesgo, The Extreme Edge at the Bottom of
the Internet of Things: A Review, IEEE Sens. J. 19 (9) (2019) 3179–3190.
[429] G. Aloi, G. Caliciuri, G. Fortino, R. Gravina, P. Pace, W. Russo, C. Savaglio,
Enabling IoT Interoperability through Opportunistic Smartphone-based Mobile
Gateways, J. Netw. Comput. Appl. 81 (2017) 74–84.
[430] X. Sun, N. Ansari, Avaptive Avatar Handoff in the Cloudlet Network, IEEE
Trans. Cloud Comput. 7 (3) (2017) 664–676.

```
[431] K.M. Rashid, J. Louis, Times-Series Data Augmentation and Deep Learning
for Construction Equipment Activity Recognition, Adv. Eng. Inform. 42 (2019)
100944.
[432] J.V. Jacobs, L.J. Hettinger, Y.-H. Huang, S. Jeffries, M.F. Lesch, L.A. Simmons,
S.K. Verma, J.L. Willetts, Employee Acceptance of Wearable Technology in the
Workplace, Applied Ergon. 78 (2019) 148–156.
[433] K.W. Ching, M.M. Singh, Wearable Technology Devices Security and Privacy
Vulnerability Analysis, Int. J. Netw. Secur. Appl. 8 (3) (2016) 19–30.
[434] D.F.S. Santos, H.O. Almeida, A. Perkusich, A Personal Connected Health System
for the Internet of Things Based on the Constrained Application Protocol,
Computers and Electrical Engineering 44.
[435] A. Martins, D. Santos, A. Perkusich, H. Almeida, IEEE 11073 and Connected
Health: Preparing Personal Health Devices for the Internet, in: Proc. of IEEE
International Conference on Consumer Electronics (ICCE), 2014.
[436] iTouch Wearables, Customer support, 2017, [Online] (Accessed March 3, 2021)
https://itouchwearables.com/pages/support.
[437] ATT, Learn About and Get Support for Wearables, 2017, [Online] (Accessed
March 3, 2021) https://www.att.com/support/article/wireless/KM1008691/.
[438] R. Snader, R. Kravets, A.F. Harris III, Cryptocop: Lightweight, Energy-Efficient
Encryption and Privacy for Wearable Devices, in: Proc. of Workshop on
Wearable Systems and Applications, 2016, 7–12.
[439] A. Ometov, Y. Bardinova, A. Afanasyeva, P. Masek, K. Zhidanov, S. Vanurin, M.
Sayfullin, V. Shubina, M. Komarov, S. Bezzateev, An Overview on Blockchain
for Smartphones: State-of-the-Art, Consensus, Implementation, Challenges and
Future Trends, IEEE Access 8 (2020) 103994–104015.
[440] O. Arias, J. Wurm, K. Hoang, Y. Jin, Privacy and Security in Internet of Things
and Wearable Devices, IEEE Trans. Multi-Scale Comput. Syst. 1 (2) (2015)
99–109.
[441] R. Fallahzadeh, H. Ghasemzadeh, Trading Off Power Consumption and Pre-
diction Performance in Wearable Motion Sensors: An Optimal and Real-Time
Approach, ACM Trans. Des. Autom. Electron. Syst. (TODAES) 23 (5) (2018)
1–23.
[442] H. Yin, N.K. Jha, A Health Decision Support System for Disease Diagnosis Based
on Wearable Medical Sensors and Machine Learning Ensembles, IEEE Trans.
Multi-Scale Comput. Syst. 3 (4) (2017) 228–241.
[443] L.C. Kourtis, O.B. Regele, J.M. Wright, G.B. Jones, Digital biomarkers for
Alzheimer’s Disease: The Mobile/Wearable Devices Opportunity, NPJ Digital
Med. 2 (1) (2019) 1–9.
[444] Z. Qin, Y. Zhang, S. Meng, Z. Qin, K.-K.R. Choo, Imaging and Fusing Time
Series for Wearable Sensor-based Human Activity Recognition, Inf. Fusion 53
(2020) 80–87.
[445] C. Bormann, A.P. Castellani, Z. Shelby, COAP: An Application Protocol for
Billions of Tiny Internet Nodes, IEEE Internet Comput. (2) (2012) 62–67.
[446] R.T. Fielding, Architectural Styles and the Design of Network-Based Software
Architectures (Ph.D. thesis), University of California, Irvine, 2000.
[447] M. Jeronimo, J. Weast, UPnP Design By Example: A Software Developer’s Guide
to Universal Plug and Play, Intel Press, 2003.
[448] H. Khattak, M. Ruta, E. Di Sciascio, CoAP-based Healthcare Sensor Networks: A
Survey, in: Proc. of 11th International Bhurban Conference on Applied Sciences
and Technology (IBCAST), 2014.
[449] M.R. Palattella, M. Dohler, A. Grieco, G. Rizzo, J. Torsner, T. Engel, L. Ladid,
Internet of Things in the 5G Era: Enablers, Architecture, and Business Models,
IEEE J. Sel. Areas Commun. 34 (3) (2016) 510–527.
[450] Fischer Connectors, Internet of Things (IoT) and Wearables, 2020, [On-
line] (Accessed March 3, 2021) https://www.fischerconnectors.com/global/en/
applications/internet-things-iot-wearables.
[451] D. Miorandi, S. Sicari, F. De Pellegrini, I. Chlamtac, Internet of Things: Vision,
Applications and Research Challenges, Ad Hoc Networks 10 (7).
[452] J. Kim, J. Lee, J. Kim, J. Yun, M2 Service Platforms: Survey, Issues, and
Enabling Technologies, IEEE Communications Surveys Tutorials 16 (1).
```

```
Computer Networks 193 (2021) 108074
```
**Aleksandr Ometov** is a Postdoctoral Research Fellow at
Tampere University (TAU), Finland. He is currently working
on H2020 MCSA ITN/EJD A-WEAR project. He received
D.Sc. (Tech) in Telecommunications and M.Sc. is Informa-
tion Technology from Tampere University of Technology
(TUT), Finland in 2018 and 2016, correspondingly. He
also holds his Specialist degree in Information Security
from Saint Petersburg State University of Aerospace Instru-
mentation (SUAI), Russia, 2013. His research interests are
wireless communications, information security, blockchain
technology and wearable applications.

**Viktoriia Shubina** is a Doctoral student at Tampere Univer-
sity (TAU), and an Early Stage Researcher at H2020 MCSA
ITN/EJD A-WEAR project. She received her Double M.Sc. in
Engineering from the University of Applied Sciences Tech-
nikum Wien, Austria, and M.Sc. in Business Informatics from
National Research University Higher School of Economics,
Russia in 2019. Topics, which interest her most are location
privacy, privacy-preserving mechanisms, indoor positioning,
and wearable technologies.

**Lucie Klus** is the Early Stage Researcher at Tampere Uni-
versity, Finland and Jaume I University, Spain as a part
of H2020 MCSA ITN/EJD A-WEAR project since Septem-
ber 2019. She received her M.Sc. and B.Sc. degrees from
Electronics and Communications at Brno University of Tech-
nology in 2019 and 2017. Her research interests include
modern approaches in wireless communications, data pro-
cessing and analytics, crowdsourcing methods and machine
learning techniques.

**Justyna Skibińska** is the Early Stage Researcher and Ph.D.
student at Brno University of Technology, Czech Republic
and Tampere University, Finland as a part of H2020 MCSA
ITN/EJD A-WEAR project. She obtained her M.Sc. and B.Sc.
degrees from Biomedical Engineering with specialization in
Computer Science and Electronics in Medicine at University
of Science and Technology in Kraków, Poland in 2018 and
2017 respectively. Her research focus is on machine learning
techniques and wearable technologies.

**Salwa Saafi** is a joint Ph.D. student at the Department
of Telecommunications at Brno University of Technology,
Czech Republic and the Unit of Electrical Engineering at
Tampere University, Finland. She received her engineer-
ing degree (2017) in telecommunications from the Higher
School of Communication of Tunis, Tunisia. Her research
interests include cellular radio access technologies, future
wireless architectures, and wearable applications.

**Pavel Pascacio** is currently an Early Stage Researcher of the
H2020 MCSA ITN/EJD A-WEAR project at the Universitat
Jaume I (Spain) and Tampere University (Finland) respec-
tively. He received his M.Sc. in Automation and Control
Engineering from Politecnico di Milano, Italy, in 2019 and a
B.Sc. in Electronics Engineering from Instituto Tecnológico
de Tuxtla Gutiérrez, México, in 2009. His main research
interests are in the areas of infrastructure-less indoor loca-
tion & positioning, machine learning, collaborative indoor
positioning systems, peer-to-peer communication and mesh
networks.

**Laura Flueratoru** is currently pursuing her joint Ph.D.
degree at University Politehnica of Bucharest and Tampere
University as part of the H2020 MSCA ITN/EJD A-WEAR
project. She received her M.Sc. degree in Electrical En-
gineering from ETH Zürich in 2019 and, prior to this,
her B.Eng. degree (with highest honors) in Electronics
and Telecommunications from University Politehnica of
Bucharest in 2017. Her main research interests are in wire-
less communications, localization systems, ultra-wideband
communications, and embedded systems.

```
Darwin Quezada Gaibor is an Early Stage Researcher and
Ph.D. student at Universitat Jaume I (Spain) and Tampere
University (Finland). He received his bachelor’s degree
in Mechatronic Engineering from Universidad Tecnológica
América, Ecuador, 2013 and his Master’s Degree in Ra-
dioengineering – GNSS receivers: Hardware and Software
from Samara National Research University, Russia, 2017.
His main interests are VoIP, Cloud Computing, Networking,
Servers, and open-source software.
```
```
Nadezhda Chukhno is an Early Stage Researcher at A-
WEAR and Doctoral Researcher at Mediterranea University
of Reggio Calabria, Italy and Jaume I University, Spain.
She graduated from RUDN University, Russia, and re-
ceived her B.Sc. in Business Informatics (2017) and M.Sc.
in Fundamental Informatics and Information technologies
(2019). Her current research activity mainly focuses on
wireless communications, 5G networks, D2D, and wearable
technologies.
```
```
Olga Chukhno is an Early Stage Researcher within H2020
MCSA ITN/EJD A-WEAR project and a Ph.D. student at
Mediterranea University of Reggio Calabria, Italy and Tam-
pere University, Finland. She received M.Sc. (2019) in
Fundamental Informatics and Information Technologies and
B.Sc. (2017) in Business Informatics from RUDN Univer-
sity, Russia. Her current research interests include wireless
communications, social networking, edge computing, and
wearable applications.
```
```
Asad Ali is an Early Stage Researcher in the H2020
MCSA ITN/EJD A-WEAR project and a Doctoral Researcher
at Tampere University, Finland, and Brno University of
Technology, Czech Republic. He pursued his B.Sc. in Elec-
trical Engineering with majors in Telecommunication from
COMSATS University Islamabad, Pakistan (2015), and M.Sc.
in Electrical Engineering from the University of Rostock,
Germany (2019). His research interests include, but are not
limited to, mmWave communication, wearable technology,
and 5G network.
```
```
Asma Channa is an Early Stage Researcher in the H2020
MCSA ITN/EJD A-WEAR project and a Doctoral Researcher
at University Politehnica of Bucharest, and Mediterranea
University of Reggio Calabria, Italy. In 2015, she graduated
from Mehran University of Engineering and Technology
Jamshoro, Pakistan with B.Sc. degree in Electronic Engi-
neering. She holds her M.Sc. degree in Electronic Systems
Engineering from the same university (2018). Her research
interests include, biomedical signal processing, wearables,
eHealth and artificial intelligence.
```
```
Ekaterina Svertoka is a Ph.D. candidate at Politehnica
University of Bucharest, Romania as part of H2020 ITN/EJD
A-WEAR project. She received her M.Sc. in Radioengi-
neering from Saint Petersburg Electrotechnical University
(LETI), Russia in 2018. Her research interests are wireless
communications and wearable technology for work safety.
```
```
Waleed Bin Qaim is an Early Stage Researcher (ESR) in the
H2020 MSCA ITN/EJD A-WEAR project. He is a double de-
gree Ph.D. student affiliated with Tampere University (TAU),
Finland and University Mediterranea of Reggio Calabria
(UNIRC), Italy. He received his M.Sc. in Computer Science
and Engineering from Koc University, Turkey in 2018.
He completed his B.Sc. in Telecommunication Engineering
from the National University of Computer and Emerging
Sciences (NUCES), Pakistan in 2011. His research interests
include Wireless Communication, IoT, Wearable Networks,
and Distributed Computing Systems.
```

```
Computer Networks 193 (2021) 108074
```
**Raúl Casanova-Marqués** is a joint-Ph.D. student at Brno
University of Technology (BUT) and Universitat Jaume I
(UJI), working as an Early Stage Researcher (ESR) within
the A-WEAR project. He graduated (2017) in Computer
Engineering at Universitat Rovira i Virgili (URV) in Spain
and he received a M.Sc. (2018) in Information and Com-
munication Technology Security from Universitat Oberta de
Catalunya (UOC), and a M.Sc. (2018) Indra Master’s in
Cybersecurity from U-tad. He is currently involved as a
researcher in several scientific projects focused on novel
cryptographic protocols for attribute-based authentication,
privacy protection mechanisms of users in electronic systems
and secure algorithms on wearable devices.

**Sylvia Holcer** is currently an Early Stage Researcher and
a Ph.D. student at Universitat Jaume I (UJI) in Castellón,
Spain with a secondment at Brno University of Technology
(BUT) in Brno, Czech Republic. She is focusing her work on
location privacy in wearables. She majored in Geoinforma-
tion for her M.Sc. and B.Sc. at Adam Mickiewicz University
in Poznań, Poland. Her primary research interests are new
technologies, machine learning, and spatial analysis.

**Joaquín Torres-Sospedra** is CEO at UBIK Geospatial So-
lutions. He has a Ph.D. since 2011 about Ensembles of
Neural Networks and Machine Learning from Universitat
Jaume I. He has authored more than 120 articles in journals
and conference proceedings. His current research interests
include indoor positioning solutions based on Wi-Fi & BLE,
Machine Learning and Evaluation. Dr. Torres-Sospedra is the
chair of the Smartphone-based track of IPIN Competition
since 2015. He is also the chair of the IPIN International
Standards Committee since 2018.

**Sven Casteleyn** received his master and Ph.D. in Computer
Science from the Vrije Universiteit Brussel, Belgium. He is
currently an associate professor at the Universidad Jaime
I, CastellÃşn, Spain, and previously held a Ramon y Cajal
(Spain) and a Marie Curie (Europe) individual post-doctoral
fellowship. Sven supervised 6 Ph.D. and over 50 master
theses. He published over 100 scientific articles in the
broad fields of the Web, mobile computing, geographical
information science and technology, and their application
fields.

**Giuseppe Ruggeri** received the master degree in electronics
engineering in 1998. In 2002 he received the Ph.D. in
electronics, computer science and telecommunications engi-
neering. He is currently assistant professor at the University
Mediterranea of Reggio Calabria. His current interests in-
clude self organizing networks, Internet of Things, Social
Internet of Things.

```
Giuseppe Araniti (Senior Member, IEEE) received the Lau-
rea degree and the Ph.D. degree in electronic engineering
from the University Mediterranea of Reggio Calabria, Italy,
in 2000 and 2004, respectively. He is currently an Assis-
tant Professor of telecommunications with the University
Mediterranea of Reggio Calabria. His major area of re-
search is on 5G/6G networks and it includes personal
communications, enhanced wireless and satellite systems,
traffic and radio resource management, multicast and broad-
cast services, device-to-device (D2D), and machine-type
communications (M2M/MTC).
```
```
Radim Burget is an Assoc. Professor at Brno University of
Technology and is heading Signal processing program at SIX
Research Centre. He has been involved in research of arti-
ficial intelligence for many years and in plenty of research
projects which include projects funded on European level,
national level or privately funded projects. Companies he
is cooperating with include Honeywell, Mitsubishi Electric,
Rapidminer, Konica-Minolta and others.
```
```
Jiri Hosek (Senior Member, IEEE) received the M.Sc. and
Ph.D. degrees in electrical engineering from the Faculty
of Electrical Engineering and Communication, Brno Univer-
sity of Technology (BUT), Czech Republic, in 2007 and
2011, respectively. He is currently an Associate Professor
and the Deputy Vice-Head for Research and Development
and International Relations at the Department of Telecom-
munications, BUT. He is also coordinating the WISLAB
Research Group, where he deals mostly with industry-
oriented projects in the area of future mobile networks, the
Internet of Things, and home automation services. He has
(co)authored more than 130 research works on networking
technologies, wireless communications, quality of service,
quality of experience, and IoT applications.
```
```
Elena Simona Lohan is a Professor at Tampere University
(TAU), Finland. She received an M.Sc. degree in electri-
cal engineering from Polytechnics University of Bucharest,
Romania, in 1997, a DEA degree (French equivalent of
master) in econometrics at Ecole Polytechnique, Paris,
France, in 1998, and a Ph.D. degree in telecommunica-
tions from Tampere University of Technology in 2003. She
is now a professor at the Electrical Engineering unit at
Tampere University, Finland and the coordinator of the
MSCA EU A-WEAR network. Her current research interests
include wireless location techniques, wearable computing,
and privacy-aware positioning solutions.
```

