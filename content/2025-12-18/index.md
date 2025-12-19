+++
title = "Fucking Ads"
date = 2025-12-18

[taxonomies]
tags = ["ads", "pihole"]
+++

I spend a non-trivial amount of time doing what I can to escape ads. Like any
normal human being, I use Firefox so I can run uBlock Origin. Back when I was
using android I was also able to use uBlock Origin with the Firefox browser. The
second-worst part of moving to iPhone is their medieval restrictions on browsers
(the first is the keyboard). At home [pi-hole](pi-hole.net) is blocking ads on
my LAN. I use [CastSponsorSkip](https://github.com/gabe565/CastSponsorSkip) to
skip sponsored ads in the middle of YouTube videos, on top of paying for YouTube
music, and therefore YouTube premium so that I don't get regular YouTube ads.

Unfortunately, there are still a few services where I still get ads. One of them
is IG. Like every other maladjusted millennial, I doom scroll on the regular.
The ads here are deceptively good at fitting into the content as the format is
the same and the indication that something is sponsored seems to be getting less
and less apparent. However, when you notice that something is sponsored, you
have the option to investigate into why you were presented with the ad,
declaring that you would prefer to see fewer ads like that, and banning all ads
from that advertiser. Of the three, I've been meticulously picking the latter
and just blocking advertisers.

{{img(src='never_again.png', alt="One-by-one", width="50%", class="center")}}

Note: While writing this I found a section of the meta ad panel that shows you
advertisers who have uploaded a list that includes your info for advertisement
purposes. It allows you to walk through each individual advertiser, one-by-one,
and disallow anyone from using that list. There are **a lot** of these.

{{ imggrid(
  cols=2,
  images=[
    "hashed_list.png",
    "list_list.png"
  ]
) }}

One thing I've noticed in the process is that blocking an advertiser is really
only blocking that single account being used to advertise. Obvious in hindsight,
but that means that if you block F1, you will still get adds from F1usa, and ads
from "DorkyEuropeanF1Driver and F1". The thing is a fucking hydra.

Another interesting note: as I've been doing some researching, I came across a
[Reddit
post](https://www.reddit.com/r/Instagram/comments/wa38w9/my_solution_for_all_the_sponsored_postsadsstories/)
where someone did the exact same thing. I wonder if they noticed any success.

Anyhow, there's some more information available to us about how we're getting
selected by advertisers. They upload "lists" that you're a part of that they can
then use to target you. Looking at these lists brings up a list of companies
that I have purchased things from and a list of companies that are just pure ad
list companies. AdParlor shows up on that list, I wonder if I can remove myself
from their list?

{{img(src='list_usage.png', alt="Meta's explainer", width="50%", class="center")}}

The first thing I need to do is disable pi-hole, or I'll never get to the
website. Once you get to the homepage, there's nothing for victims, just brands
and agencies. At the _very_ bottom of the page, to the far right, there's a
privacy policy!

> AdParlor and/or its partners reserve their rights to use cookies to track
> individual responses or views of advertisements, and use this information to
> help predict what other advertisements may be of interest to consumers and
> enable the receipt of customized advertisements or content. These cookies
> contain no personally identifiable information. The cookies may reflect
> de-identified demographic or other data linked to data you voluntarily have
> submitted to us, such as your email address, that we may share with any third
> party, solely in hashed, non-human readable form. To learn about how you can
> opt-out of the receipt of cookies, please visit http://www.aboutads.info/
> choices and to learn more about cookies in general, please visit
> http://www.cookiecentral.com. See more information about changing cookie
> preferences below in Use of Information and User Data section of policy.

Oh, good for them. Reserving their rights to track me. And then pointing me to
some bullshit ad apologist website made by the "Digital Advertising Alliance".
Get fucked. Most of this policy is dedicated to those with accounts here, not
victims. However, there seems to be a section that might be relevant.

{{img(src='privacy_rights.png', alt="Privacy Rights?", width="50%", class="center")}}

And this is the problem. I have no idea what information they have. What email
address are they using? I've had dozens over the years. They're likely all
linked anyway, but it's pretty apparent that they will delete the minimum
possible amount. On the meta side, I have no idea why I'm in that list, on the
ad list side, I have no idea what information they have. How the _fuck_ do I
exercise my rights?

I guess I'll keep telling meta to stop using lists and send emails into the
void.
