Title: This Week in Rust 273
Number: 273
Date: 2019-02-12
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

# Updates from Rust Community

## News & Blog Posts
* [Are you still using 'println' in Rust for debugging?](https://blog.knoldus.com/are-you-still-using-println-in-rust-for-debugging/).

# Crate of the Week

This week's crate is [log-derive](https://crates.io/crates/log-derive), a procedural macro to log function outputs. Thanks to [elichai2](https://users.rust-lang.org/t/crate-of-the-week/2704/482) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

- [raft: Convert `Storage::entries`'s `max_size` argument to `Option<u64>`](https://github.com/pingcap/raft-rs/issues/98)
- [TiKV: Convert trait objects to `dyn` syntax for Rust 2018](https://github.com/tikv/tikv/issues/4197)
- [TiKV: Remove all the `extern crate`s for Rust 2018](https://github.com/tikv/tikv/issues/4196)
- [TiKV: Add tcmalloc support to the tikv_alloc crate](https://github.com/tikv/tikv/issues/4191)

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

157 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2019-01-28..2019-02-04

* [HirIdification: add key HirId methods](https://github.com/rust-lang/rust/pull/58090)
* [don't panic when accessing enum variant ctor using `Self` in match](https://github.com/rust-lang/rust/pull/58007)
* [use LLVM intrinsics for saturating add/sub](https://github.com/rust-lang/rust/pull/58003)
* [add MOVBE x86 CPU feature](https://github.com/rust-lang/rust/pull/57999)
* [NVPTX target specification](https://github.com/rust-lang/rust/pull/57937)
* [fix bug in integer range matching](https://github.com/rust-lang/rust/pull/57978)
* [unused variable suggestions apply on all patterns](https://github.com/rust-lang/rust/pull/57899)
* [add information to higher-ranked lifetimes conflicts error messages](https://github.com/rust-lang/rust/pull/57901)
* [rustc: use multiple threads by default](https://github.com/rust-lang/rust/pull/57948)
* [misc performance tweaks](https://github.com/rust-lang/rust/pull/57916)
* [simplify `ConstValue::ScalarPair`](https://github.com/rust-lang/rust/pull/57442)
* [mark `str::trim*` functions as `#[must_use]`](https://github.com/rust-lang/rust/pull/57106)
* [override `VecDeque`'s `Iter::try_fold`](https://github.com/rust-lang/rust/pull/57974)
* [introduce `into_raw_non_null` on `Rc` and `Arc`](https://github.com/rust-lang/rust/pull/57934)
* [implement `Weak::`{`strong_count`, `weak_count`}](https://github.com/rust-lang/rust/pull/56696)
* [rename `iter::unfold` to `iter::from_fn` and remove explicit state](https://github.com/rust-lang/rust/pull/58062)
* [stabilize `std::error::Error::type_id`](https://github.com/rust-lang/rust/pull/58048)
* [stabilize `split_ascii_whitespace`](https://github.com/rust-lang/rust/pull/58047)
* [cargo: fix overlapping progress with stdout](https://github.com/rust-lang/cargo/pull/6618)
* [cargo: improve progress bar flickering](https://github.com/rust-lang/cargo/pull/6615)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: e] [Generic integers](https://github.com/rust-lang/rfcs/pull/2581).
* [disposition: e] [Accept semicolons as item-like](https://github.com/rust-lang/rfcs/pull/2479).

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Stabilize TryFrom and TryInto with a convert::Infallible empty enum](https://github.com/rust-lang/rust/pull/58302).
* [disposition: merge] [Tracking issue for str::as_mut_ptr](https://github.com/rust-lang/rust/issues/58215).
* [disposition: merge] [Stabilize slice_sort_by_cached_key](https://github.com/rust-lang/rust/pull/58074).
* [disposition: merge] [deprecate before_exec in favor of unsafe pre_exec](https://github.com/rust-lang/rust/pull/58059).
* [disposition: merge] [Stabilize linker-plugin based LTO (aka cross-language LTO)](https://github.com/rust-lang/rust/pull/58057).
* [disposition: merge] [Tracking issue for std::iter::successors](https://github.com/rust-lang/rust/issues/58045).
* [disposition: merge] [Tracking issue for Option::copied](https://github.com/rust-lang/rust/issues/57126).
* [disposition: merge] [Tracking issue for std::ptr::hash](https://github.com/rust-lang/rust/issues/56286).
* [disposition: merge] [Rename `MaybeUninit` to `MaybeUninitialized`](https://github.com/rust-lang/rust/pull/56138).
* [disposition: merge] [Tracking issue for std::iter::from_fn](https://github.com/rust-lang/rust/issues/55977).

## New RFCs

* [RFC changing the overflow behavior for usize in release builds to panic](https://github.com/rust-lang/rfcs/pull/2635).
* [#[ffi_returns_twice]](https://github.com/rust-lang/rfcs/pull/2633).

# Upcoming Events

### Online

* [Feb 13. Rust Events Team Meeting on Telegram](https://t.me/joinchat/EkKINhHCgZ9llzvPidOssA).
* [Feb 20. Rust Community Team Meeting on Discord](https://discordapp.com/channels/442252698964721669/443773747350994945).
* [Feb 25. Rust Community Content Subteam Meeting on Discord](https://discordapp.com/channels/442252698964721669/443773747350994945).
* [Feb 27. Rust Events Team Meeting on Telegram](https://t.me/joinchat/EkKINhHCgZ9llzvPidOssA).

### Asia Pacific

* [Feb 13. Melbourne, AU - Melbourne hack night](https://www.meetup.com/Rust-Melbourne/events/257974991/).
* [Feb 16. Chennai, IN - Rust Chennai meetup](https://www.meetup.com/mad-rs/events/258822338/).

### Europe

* [Feb 12. Villeurbanne, FR - TupperRust](https://tupperrust.github.io).
* [Feb 18. Karlsruhe, DE - Karlsruhe Rust Hack and Learn](https://www.meetup.com/Rust-Hack-Learn-Karlsruhe/events/258728236/).
* [Feb 20. Berlin, DE - Berlin Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/rjgkhqyzdbbc/).

### North America

* [Feb 12. Utah, US - Utah Rust monthly meetup](https://www.meetup.com/utahrust/events/257819656/).
* [Feb 13. Ciudad de México, MX - Study group RustMX](https://www.meetup.com/es/Rust-MX/).
* [Feb 14. Columbus, US - Columbus Rust Society](http://www.meetup.com/columbus-rs/).
* [Feb 14. San Diego, US - San Diego Rust](http://meetu.ps/c/2vF0G/4DXV4/a).
* [Feb 20. Chicago, US - Chicago Rust Meetup - Property-Based Testing in Rust](https://www.meetup.com/Chicago-Rust-Meetup/events/257469240/).
* [Feb 20. Vancouver, CN - Vancouver Rust meetup](https://www.meetup.com/Vancouver-Rust/events/).
* [Feb 21. Arlington, US - Rust DC—Learn+Try: Custom Redis Datastructures](https://www.meetup.com/RustDC/events/257969733).
* [Feb 25. Durham, US - Triangle Rustaceans](https://www.meetup.com/triangle-rustaceans/).
* [Feb 27. Ann Arbor, US - Ann Arbor Rust Meetup](https://www.meetup.com/Ann-Arbor-Rust-Meetup/).
* [Feb 27. Ciudad de México, MX - Study group RustMX](https://www.meetup.com/es/Rust-MX/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Software Engineer at Discord, San Francisco, US](https://discordapp.com/jobs/4200751002).
* [Network Engineer at NearProtocol, San Francisco, US](https://nearprotocol.com/careers/?gh_jid=4205573002).
* [Navitia Software Engineer at Kisio Digital, Paris, FR](https://www.welcometothejungle.co/companies/kisio-digital/jobs/rust-c-developpeur-h-f_paris).
* [Rust web developer at Impero, Denmark/remote](https://impero.com/job/full-stack-web-developer-rust/)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

This time, we have two quotes for the price of one:

> The borrow checker breaks you down so that it can build you back up, stronger and more resilient than you once were. It also had me do all sorts of weird things like catch flies with chopsticks and scrub counters to a polish.

– /u/bkv on [/r/rust](https://www.reddit.com/r/rust/comments/ampvvt/as_a_new_selftaught_student_to_programming_this/efnw35o/)

> I always think of borrowck as an angel sitting on your shoulder, advising you not to sin against the rules of ownership and borrowing, so your design will be obvious and your code simple and fast.

– llogiq on [/r/rust](https://www.reddit.com/r/rust/comments/ampvvt/as_a_new_selftaught_student_to_programming_this/efo074d)

Thanks to [Christopher Durham](https://users.rust-lang.org/t/twir-quote-of-the-week/328/617) for the suggestion!

[Please submit your quotes for next week](http://users.rust-lang.org/t/twir-quote-of-the-week/328)!

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [Flavsditz](https://github.com/Flavsditz).*

<small>[Discuss on r/rust]().</small>