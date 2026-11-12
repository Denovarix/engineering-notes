# AFRT: software that adapts to you without reading you

We are building an operating system in India. Not a skin, not a theme. A full business OS called DNX OS, with AI that runs on the device.

Today I want to explain one thing inside it: **AFRT, Adaptive Feedback Response Technology.** It is coming in DNX OS, and it is opt-in.

![AFRT: software that adapts to you without reading you](https://raw.githubusercontent.com/Denovarix/afrt/main/assets/afrt-1.jpg)

## The problem with "smart" software

Every smart product learns about you the same way. It reads everything you do. Your files, your messages, your searches.

I don't want that for my company, and I don't want it for yours. But I do want software that gets better at fitting the person using it. So the question we asked was simple: how much can a system adapt if it is never allowed to see content?

Our answer is one rule: **count, never read.**

## What AFRT counts

- **Which app was opened.** Mail, Files, Sheets. The name of the app, nothing inside it.
- **Which screen or settings page.** So the next update can put what you use within reach.
- **Which theme is in use.** So defaults match what people actually choose.
- **That the microphone opened something.** That voice was used. Never what was said.
- **The hour of day.** Twenty-four counters. Nothing finer than the hour.

That is the whole list. Each entry is a name and a number.

![AFRT counts. It does not read.](https://raw.githubusercontent.com/Denovarix/afrt/main/assets/afrt-3.jpg)

## What it can never keep

This part matters more than the list above.

- **File names.** An event has to be a short lowercase identifier from a fixed set of kinds. A file name is refused.
- **Messages, searches, anything typed.** There is no event kind for content at all.
- **Your name or a device ID.** Neither is in what it stores or exports.
- **Unlimited history.** At most 400 distinct things are counted, so the record cannot grow without end.

These are rules in the code, with tests that try to push content in and check that it is refused. It is not a policy promise that someone can quietly change.

![What it can never keep](https://raw.githubusercontent.com/Denovarix/afrt/main/assets/afrt-4.jpg)

## You hold the switch

- It is **off until you switch it on**, in Settings, under Privacy & security.
- You can **read exactly what is held**, on one screen, in plain words, and save it to a file.
- You can **wipe it in one click**. Switching it off wipes it too. Off means nothing is held.
- **Nothing leaves the PC.** AFRT sends nothing anywhere. Sharing with us would be a separate, later step, and it must show you the same summary first.

![You hold the switch](https://raw.githubusercontent.com/Denovarix/afrt/main/assets/afrt-5.jpg)

## What it does not do yet

I would rather say this plainly.

- It does not rearrange the interface for you today.
- Nova, the assistant in DNX OS, does not learn from it today.
- It is not in a released build. DNX OS opens its beta in December 2026 and launches in January 2027.

What exists is the counting, the limits, the switch, the summary and the wipe. The adapting comes next, and it will be built on top of data this small on purpose.

## Why we are telling you before it ships

Because the design is the product. If a privacy feature only sounds good after launch, it was marketing. If you can read the rules before it exists and hold us to them, it is engineering.

- The design, in the open: [github.com/Denovarix/afrt](https://github.com/Denovarix/afrt)
- The page on Hugging Face: [Denovarix/afrt](https://huggingface.co/spaces/Denovarix/afrt)
- DNX OS: [denovarix.com/dnx-os](https://denovarix.com/dnx-os/)
- Beta programme: [denovarix.com/beta](https://denovarix.com/beta/)

*Sourav De, founder, Denovarix Technologies LLP. Write to us at hello@denovarix.com.*
