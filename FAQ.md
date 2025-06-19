# FAQ

## Table of Contents

### Strategy & Approach
- [What actual force do you have over AMD?](#actual-force)
- [Why not target NVIDIA directly?](#why-amd)  
- [Doesn't AMD already know all of this?](#amd-knows)
- [Why shareholder activism instead of working with AMD directly?](#why-shareholder-activism)
- [What happens if AMD ignores the shareholder resolution?](#if-ignored)

### Technical Context
- [What specific technical problems need to be fixed?](#technical-problems)
- [How is AMD's ROCm different from CUDA?](#rocm-vs-cuda)
- [What would success look like for developers?](#success-metrics)

### Participation & Getting Involved
- [How can I help if I'm not a developer or investor?](#how-to-help)
- [Do I need to buy AMD stock to participate?](#need-stock)
- [What's the timeline for this campaign?](#timeline)
- [How will I know if this campaign is making progress?](#tracking-progress)

### About the Campaign
- [How is this different from online petitions?](#vs-petitions)
- [Who is behind this campaign?](#who-behind)

---

## Strategy & Approach

<a id="actual-force"></a>
## Q: What actual force do you have over AMD? How can a few people change a billion-dollar company?

**A:**

We're not just making noise—we're using formal shareholder activism, which is fundamentally different from internet petitions.

**The barrier is surprisingly low:** Anyone owning just $2,000 of AMD stock for one year can file a shareholder resolution. We already meet these requirements.

**Why resolutions matter:** Unlike petitions, shareholder resolutions are formal corporate governance that:
- Get mandatory inclusion in proxy statements sent to all shareholders
- Require board response and public disclosure
- Generate media coverage because they're real corporate actions, not just online campaigns
- Even minority votes of 10-20% create significant pressure and force management attention

**Real precedent:** Engine No. 1 successfully changed ExxonMobil's board with only 0.02% ownership by combining technical credibility with strategic activism.

Our unique advantage is combining developer expertise with investor pressure—making our demands technically credible and financially legitimate.

For detailed explanation of our shareholder activism strategy, see [Shareholder Activism: How You Can Force Real Change](Activism.md).

<a id="why-amd"></a>
## Q: Why not target NVIDIA directly? Isn't NVIDIA the real problem? Why focus on AMD when they already support open source?

**A:**

NVIDIA's CUDA monopoly is the core problem—it creates vendor lock-in, inflates prices, and blocks open AI/scientific computing. We absolutely want open GPU computing free from single-vendor control.

However, NVIDIA only responds to real competition, not public pressure. Years of calls to "open up CUDA" have been ignored because their monopoly works and their platform "just works."

AMD is the only realistic challenger with both the hardware and open-source commitment. But AMD's current "openness" isn't enough:

- Software experience (drivers, libraries, ease of use) lags far behind NVIDIA
- Developers face broken workflows, missing features, and limited support
- Community verdict: "Open source" is just marketing unless tools actually work

### Why focus on AMD?

NVIDIA's monopoly will only break when a credible, open alternative exists. The fastest path is pushing AMD to deliver on their potential—fixing software, expanding support, and earning developer trust.

Our campaign demands execution, not promises. We're pushing AMD to be truly competitive, not just "open."

### If AMD delivers, everyone wins:

- Prices drop and the "CUDA tax" disappears
- Open science and AI become accessible to more people
- NVIDIA is forced to compete or open up

### Bottom line:

AMD is the only company with a realistic path to break NVIDIA's monopoly—but only if they fix what's broken. When AMD wins, we all win.

<a id="amd-knows"></a>
## Q: Doesn't AMD already know all of this? Why should an external campaign be necessary?

**A:**

It's true—AMD's leadership understands the CUDA monopoly, the market opportunity, and the need for a competitive open-source software stack. They talk about it in interviews, investor calls, and press releases. They know what needs fixing.

So why is outside pressure still needed?

**Knowing ≠ Doing.** Big organizations often struggle to turn knowledge into action. AMD has known about these problems for years—but progress has been slow and inconsistent.

**Credibility Gap.** Developers and investors have been burned by broken promises and missed timelines. There's a lack of trust that AMD will deliver without public accountability.

**Internal Pressures.** Like any large company, AMD has shifting priorities, competing departments, and budget constraints. It's easy for crucial software work to be delayed or cut—unless there's a strong outside signal that the world is watching.

**Independent Oversight Creates Results.** Think of credit rating agencies: every company knows it should manage its debt, but ratings still matter—because external scrutiny affects access to capital, board decisions, and even executive compensation. The same is true for open software at AMD: public, independent evaluation makes it a top priority, not just an internal talking point.

**Proven Track Record.** In tech, real change—open drivers, better standards, security audits—almost always follows sustained, external, community or investor pressure. It's rarely just the result of internal insight.

**In short:**
We're not here to "educate" AMD. We're here to create the public, independent accountability that finally moves the needle. Even when management knows the right answer, external pressure and oversight are what turn promises into progress.

<a id="why-shareholder-activism"></a>
## Q: Why shareholder activism instead of working with AMD directly?

**A:**

We've tried the traditional approaches—developer feedback, community forums, open source contributions, and direct outreach to AMD. These efforts have yielded limited results because they lack formal leverage.

**Shareholder activism is different because it:**
- Creates legal obligations (resolutions must be included in proxy statements)
- Forces board-level attention (can't be delegated to lower-level managers)
- Generates public accountability (voting results become public record)
- Provides ongoing leverage (annual meetings create recurring pressure)

**We're not abandoning collaboration**—we're adding accountability. The goal is to make AMD's existing promises credible by creating external verification and pressure.

Think of it as "trust but verify" for corporate commitments.

<a id="if-ignored"></a>
## Q: What happens if AMD ignores the shareholder resolution?

**A:**

Even if AMD's management opposes our resolution, the process itself creates multiple pressure points:

**Immediate Impact:**
- Resolution gets included in proxy materials sent to all shareholders
- AMD must provide an official response explaining their position
- Media coverage highlights the issues and AMD's response
- Analysts and institutional investors pay attention

**Ongoing Pressure:**
- We can file similar resolutions annually until issues are addressed
- Voting results become public benchmarks of shareholder sentiment
- Poor responses damage AMD's credibility with developers and investors
- Success builds momentum for future campaigns

**Historical Pattern:**
Most successful shareholder campaigns don't win on the first vote—they build pressure over time. Engine No. 1 spent months building their case before their ExxonMobil victory.

Even "losing" votes of 10-20% often trigger management action because they signal serious problems that can't be ignored.

---

## Technical Context

<a id="technical-problems"></a>
## Q: What specific technical problems need to be fixed?

**A:**

The problems fall into several key categories:

**1. Driver Stability & Installation**
- Frequent black screens, timeouts, and crashes on Windows
- Fragile installation process that breaks with Windows updates
- Poor compatibility with multi-monitor setups and third-party tools

**2. Limited Hardware Support**
- ROCm only supports "blessed" GPUs, often dropping consumer cards
- Missing support for widely-available RX 6000/7000 series
- Short support lifecycles compared to NVIDIA

**3. Software Ecosystem Gaps**
- Missing Windows support for ROCm (ML development mostly happens on Windows)
- Incomplete library support (FlashAttention, LoRA, many JAX features)
- Poor compatibility with popular ML frameworks out of the box

**4. Documentation & Tooling**
- Unclear documentation compared to CUDA
- Missing beginner-friendly tutorials and migration guides
- Limited debugging and profiling tools

**5. Developer Trust**
- Years of broken promises have created skepticism
- Poor communication about roadmaps and deprecation plans
- Lack of transparent progress reporting

For detailed technical priorities, see our [Developer Priorities Document](Priorities.md).

<a id="rocm-vs-cuda"></a>
## Q: How is AMD's ROCm different from CUDA, and why does it matter?

**A:**

**ROCm (AMD's platform):**
- Open source and vendor-neutral
- Supports HIP (similar to CUDA) and other standards
- Works on AMD GPUs and aims for broader hardware support
- Smaller ecosystem with gaps in libraries and tools

**CUDA (NVIDIA's platform):**
- Proprietary and NVIDIA-only
- Mature ecosystem with extensive libraries and tools
- "Just works" experience that developers trust
- Creates vendor lock-in—code written for CUDA only runs on NVIDIA

**Why this matters:**
NVIDIA's monopoly allows them to charge premium prices (the "NVIDIA tax") and control the direction of AI/scientific computing. A competitive, open alternative would:
- Drive down GPU prices through competition
- Prevent vendor lock-in for researchers and companies
- Enable innovation that isn't controlled by a single company
- Make AI and scientific computing more accessible

The technical capabilities exist—AMD's hardware is competitive. The missing piece is the software ecosystem and developer trust that makes ROCm a viable alternative to CUDA.

<a id="success-metrics"></a>
## Q: What would success look like from a developer perspective?

**A:**

**Short-term (6-12 months):**
- Stable drivers that don't break with routine updates
- ROCm working reliably on popular consumer GPUs (RX 6000/7000 series)
- Clear installation process with good error messages and recovery

**Medium-term (1-2 years):**
- ROCm for Windows with major ML frameworks (PyTorch, TensorFlow)
- Popular libraries working out of the box (FlashAttention, Triton, etc.)
- Documentation quality matching CUDA's level of detail and clarity

**Long-term (2-3 years):**
- Developers choosing AMD for new projects, not just grudgingly accepting it
- "It just works" reputation comparable to NVIDIA's
- Vibrant ecosystem of tools, tutorials, and community contributions

**Market indicators:**
- Increased AMD GPU sales in AI/ML segments
- More startups and research groups choosing AMD
- Competitive pricing pressure on NVIDIA
- Cross-platform ML frameworks using AMD as first-class backend

---

## Participation & Getting Involved

<a id="how-to-help"></a>
## Q: How can I help if I'm not a developer or investor?

**A:**

There are many ways to contribute:

**Spread Awareness:**
- Share the campaign on social media (#UnlockGPU)
- Discuss with friends in tech, finance, or academia
- Write about the issues on your blog or LinkedIn

**Provide Use Cases:**
- Share stories about GPU computing challenges you've faced
- Explain how vendor lock-in affects your work or studies
- Help document real-world impacts of the current situation

**Join the Community:**
- Follow project updates and vote on priorities
- Participate in discussions about campaign strategy
- Connect us with relevant experts or organizations

**Financial Support:**
- Consider buying AMD stock (even small amounts help)
- Support organizations working on open standards
- Donate to open source GPU computing projects

Every voice matters—this campaign's strength comes from broad, diverse support across the tech community.

<a id="need-stock"></a>
## Q: Do I need to buy AMD stock to participate?

**A:**

**No, stock ownership isn't required to participate** in most aspects of the campaign. You can contribute by spreading awareness, providing technical feedback, and supporting the community.

**However, owning AMD stock does provide additional leverage:**
- You can vote on shareholder resolutions
- Your voice carries weight as an actual owner
- It aligns your financial interests with the campaign's success

**The barrier is low:** You only need $2,000 of AMD stock held for one year to file formal resolutions, but any amount of ownership gives you voting rights.

**Alternative approaches:**
- Many institutional investors (pension funds, ETFs) hold AMD stock on your behalf
- You can influence their voting through shareholder advocacy organizations
- Focus on technical contributions and community building

Stock ownership amplifies your voice, but the campaign's success depends on broad participation from the entire tech community.

<a id="timeline"></a>
## Q: What's the timeline for this campaign?

**A:**

**Immediate (2024-2025):**
- Build developer coalition and document technical priorities
- Recruit institutional investor allies
- Prepare shareholder resolution for AMD's 2025 annual meeting

**Near-term (2025-2026):**
- File and campaign for shareholder resolution
- Generate media coverage and industry attention
- Track AMD's response and any commitments made

**Medium-term (2026-2027):**
- Monitor progress on AMD's commitments
- File follow-up resolutions if needed
- Measure improvements in developer experience and market share

**Long-term (2027+):**
- Evaluate success and consider expanding to other companies
- Support ongoing open GPU computing initiatives
- Maintain pressure for continued progress

**Key milestone:** AMD's annual shareholder meeting (typically May) is the focal point for formal resolutions, but campaign activities happen year-round.

<a id="tracking-progress"></a>
## Q: How will I know if this campaign is making progress?

**A:**

We're committed to transparent progress tracking:

**Public Metrics:**
- Shareholder resolution vote counts and percentages
- AMD's official responses to resolutions and developer feedback
- Technical improvements measured against our [Priorities Document](Priorities.md)
- AMD GPU market share in AI/ML segments

**Regular Updates:**
- Quarterly progress reports on campaign activities
- Technical assessments of ROCm and driver improvements
- Media coverage and industry response tracking
- Community feedback and developer sentiment surveys

**Measurable Outcomes:**
- Reduced developer complaints about installation and stability
- Increased adoption of AMD GPUs in ML/AI projects
- More competitive pricing in GPU markets
- Improved developer documentation and support

**Community Verification:**
- Independent testing and benchmarking by community members
- Open tracking of issues and resolution status
- Regular community calls and feedback sessions

Progress will be visible, measurable, and independently verifiable—not just corporate promises.

---

## About the Campaign

<a id="vs-petitions"></a>
## Q: How is this different from online petitions?

**A:**

**Online petitions:**
- Informal requests with no legal status
- Easy to ignore with no consequences
- Often lack specific, actionable demands
- Generate temporary attention but rarely lasting change

**Shareholder activism:**
- Legally binding process with SEC oversight
- Creates formal obligations for corporate response
- Forces board-level attention and public disclosure
- Provides ongoing leverage through annual meetings
- Combines financial pressure with technical credibility

**Our unique approach:**
- Developer expertise makes demands technically credible
- Investor participation provides financial leverage
- Public campaign builds media pressure and accountability
- Specific, measurable demands with clear success criteria

This isn't just asking politely—it's using the formal mechanisms of corporate governance to create real pressure for change.

<a id="who-behind"></a>
## Q: Who is behind this campaign?

**A:**

This campaign is led by a coalition of GPU developers and AMD shareholders who are frustrated with the slow progress on software ecosystem improvements.

**Leadership includes:**
- Developers with years of experience fighting ROCm installation issues
- Investors who see unrealized value in AMD's hardware capabilities
- Researchers blocked by vendor lock-in in scientific computing
- Open source advocates working on GPU computing standards

**Not affiliated with:**
- AMD competitors (this isn't about helping NVIDIA)
- Short sellers or financial manipulators
- Any specific company or organization with conflicting interests

**Our motivation:**
We believe AMD has incredible hardware potential being held back by solvable software problems. We're using our dual roles as developers and shareholders to push for the improvements that will benefit everyone.

**Transparency commitment:**
All campaign activities, funding sources, and conflicts of interest are disclosed publicly. This is about improving the ecosystem, not advancing hidden agendas.

