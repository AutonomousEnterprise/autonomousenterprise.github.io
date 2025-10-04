---
published: false
date: 2025-10-04
title: The Large Transformation Antipattern
author: djankov
---
In 2011, the German supermarket giant Lidl set out to modernize its technology backbone. The goal was ambitious: replace its legacy inventory management system with a cutting-edge enterprise resource planning platform based on SAP HANA. The vision was to streamline operations, gain real-time insights, and unlock efficiencies across its sprawling retail empire. Seven years later, the project was abruptly abandoned. More than half a billion euros had been sunk into the initiative, with nothing to show for except a bruised reputation and a fractured relationship between technology and the business. For Lidl, the consequences were immediate and severe. For the business world, the failure stands as one of the most striking reminders of the risks that accompany large-scale technology transformations.

## The Why and the How of a Large Technology Transformation

Large technology transformations are born out of necessity. Organizations embark on them when existing systems or operating models become so constraining that they impede growth, efficiency, or competitiveness. The timing is almost always linked to a pivotal business moment: the collapse of a legacy system under the weight of technical debt, a merger that demands the integration of disparate platforms, a new regulatory regime requiring traceability and transparency, or the adoption of a business model that the old systems cannot support. In every case, the organization seeks not an incremental improvement but a step change in capability.

The prototypical example of such a transformation is the implementation of an enterprise resource planning system, designed to integrate finance, supply chain, HR, and more into a single unified platform. Other examples include core banking system replacements, large-scale cloud migrations, and customer relationship management platform rollouts. In scope, scale, and ambition, these are the corporate equivalent of open-heart surgery – lifesaving if successful, catastrophic if not.

Due to their scale, transformations are not run as ordinary IT projects. They are organized as enterprise-wide programs, with layers of governance and oversight. A steering committee, usually comprising senior executives from both business and technology, is set up to provide strategic direction and make decisions on scope, funding, and trade-offs. A program management office coordinates day-to-day execution, manages risks, and tracks progress against milestones. On paper, this governance model creates clarity and accountability. In practice, it often struggles with slow decision-making, diffusion of responsibility, and the perennial challenge of aligning business and IT interests.

Methodology plays a decisive role. While traditional waterfall methodologies were once the standard, their rigidity is often ill-suited for the uncertainty of large transformations. Consequently, many organizations now adopt hybrid approaches or aim for more agile frameworks. However, scaling agile practices across a massive program presents its own challenges in coordination and alignment. Frameworks such as SAFe attempt to bring order to the chaos, but they often reintroduce the very bureaucracy agile sought to eliminate. Coordination across hundreds of agile teams requires new governance layers, which can slow decision-making as much as waterfall once did. Many organizations end up in a hybrid state: agile at the edges, waterfall at the core. The result can be the worst of both worlds: the rigidity of waterfall combined with the overhead of agile.

Large transformations are typically done in phases, beginning with strategy and discovery, where the business case, vision, and high-level roadmap are defined. This is followed by design, where technical architectures and process blueprints are created. The build phase involves system configuration, customization, integration, and testing. Deployment brings the system into production, either through a phased rollout or a “big bang” launch. Finally, adoption and optimization attempt to realize the intended benefits and make continuous improvements. Each phase comes with its own risks. Strategy phases often oversimplify; design phases underestimate complexity; build phases encounter integration challenges; deployments introduce operational risk; adoption falters if employees resist. The sheer length of the journey, often five to seven years, creates opportunities for scope drift, leadership turnover, and strategic priorities to change midstream.

## Anatomy of Failure

The sobering truth is that the majority of large technology transformations fail to meet their objectives. Some collapse entirely, as Lidl’s did. Others limp across the finish line, but over budget, behind schedule, and with compromised scope. Industry studies consistently point to a failure rate that should give any executive pause.

The reasons are manifold and deeply intertwined. One of the most fundamental is the failure to achieve strategic alignment. Too often, transformations are treated as “IT projects” rather than business-wide initiatives. When technology goals are divorced from business outcomes, projects drift, executive support wanes, and the transformation loses its reason for being. Unrealistic expectations compound the problem. Initial business cases are often overly optimistic, underestimating cost and effort, while overpromising benefits. As the program unfolds, stakeholders demand additional features. Without rigorous change control, scope creep becomes inevitable, swelling budgets and delaying delivery.

Leadership plays an equally decisive role. Many programs suffer from inadequate sponsorship. The executive nominally responsible may not be senior enough to command resources or may fail to engage actively, leaving the project rudderless in moments of crisis. Meanwhile, the people side of the change is frequently neglected. Employees are not prepared for new ways of working, resistance is underestimated, and communication is sporadic and top-down. The result is poor adoption, and without adoption, even the best system cannot deliver value.

Weak governance and planning exacerbate the situation. Program structures may look robust on paper, but in reality decision-making is slow, risks are poorly managed, and dependencies are not understood. These problems are not merely technical but organizational, cultural, and political. Preventing scope creep requires saying “no” to powerful stakeholders. Ensuring adoption requires changing ingrained habits. Such challenges are far harder than solving technical issues.

The consequences of failure are far reaching. On the technology side, organizations are often left with partially implemented systems that must coexist with legacy platforms, creating greater complexity and technical debt. For the IT organization, failure damages credibility and morale, reinforcing perceptions of IT as a cost center incapable of enabling business change. For the broader business, the stakes are higher still. Financial losses can reach hundreds of millions. Strategic opportunities are missed, leaving firms exposed to more agile competitors. Botched go-lives disrupt operations, alienate customers, and erode trust with suppliers. In some cases, as with Target Canada or the TSB Bank migration, the fallout can alter the trajectory of an entire business. High-profile failures in government projects, such as HealthCare.gov or Queensland Health’s payroll system, reveal that even public institutions are not immune to reputational and political damage.

|     |     |
| --- | --- |
| **Issue** | **Description** |
| Poor Strategic Alignment | Treating the transformation as an IT project rather than a business-wide initiative causes loss of direction and executive support. |
| Lack of Clear Vision | Absence of shared goals and stretch targets grounded in data creates confusion and unambitious outcomes. |
| Inadequate Leadership and Sponsorship | Sponsors lack authority or engagement, leaving the program without decisive guidance and support. |
| Unrealistic Expectations and Scope Creep | Overly optimistic business cases and uncontrolled addition of new requirements inflate costs and timelines. |
| Ineffective Governance | Weak PMO, lack of empowered decision-makers, and fragmented leadership delay resolution and reduce accountability. |
| Inadequate Change Management | Absence of strategies for adoption, training, and behavioral change leads to poor user acceptance. |
| Change Resistance | Organizational inertia, cultural resistance, and “if it isn’t broke” mindsets undermine adoption. |
| Ineffective Communication | Top-down, infrequent communication erodes trust and fails to prepare employees for new ways of working. |
| Siloed Collaboration | Insufficient alignment between business and IT leads to incorrect prioritization, missing requirements, and poor integration. |
| Poor Planning | Undefined scope, ambiguous business case, and weak resource planning undermine transformation efforts. |
| Complex Interdependencies | Failure to map and manage dependencies across initiatives amplifies cascade risks and surprises. |
| Data and Testing Issues | Poor quality data, skimped validation, and insufficient testing result in production defects and unrealistic expectations. |
| Stakeholder Misalignment | Conflicting incentives, trust deficits, poor communication, and misaligned evaluation criteria hinder collaboration. |
| Black Swan Risk | Skewed risks mean a small number of projects face extreme overruns, sometimes 200% over cost and 70% over schedule. |
| Sector-Specific Risks | In public sector projects, cost overruns above 25% are common, with risk increasing by 4.2 percentage points per year of duration. |

## What Went Wrong at Lidl

The Lidl case encapsulates many of these dynamics. The choice of SAP HANA was not inherently flawed. Indeed, it was a robust and widely adopted platform. The problems arose in how Lidl sought to deploy it. The retailer’s existing inventory management system was heavily customized and central to its operational model. Rather than adapting its processes to fit SAP’s standardized best practices, Lidl insisted on bending the software to replicate its idiosyncratic workflows. This decision set the stage for spiraling customization, mounting complexity, and soaring costs. It was a textbook violation of one of the cardinal principles of ERP implementation: adapt processes to the system, not the other way around.

Leadership also underestimated the scale and complexity of the change. The belief that a decades-old bespoke system could be mirrored within a standardized package revealed a profound misunderstanding of what the transformation entailed. At the governance level, the project was allowed to drift for seven years, consuming half a billion euros before being abandoned. A stronger steering committee would have forced a strategic decision much earlier: either commit to changing the business processes or reconsider the platform. Instead, sunk cost thinking and inertia prevailed.

Another factor was the heavy reliance on consultants. While external expertise is indispensable in projects of this scale, over-reliance risks creating a knowledge gap within the organization and ceding too much influence to vendor agendas. In Lidl’s case, escalating consultant fees were a visible symptom of a project losing control. Ultimately, the failure was not about the technology itself but about organizational misalignment, governance breakdowns, and the unwillingness to adapt core processes. It was a failure of transformation leadership, not of software engineering.

## Guidance for the C-Suite

The lessons for senior executives are clear. Large technology transformations are not technical endeavors to be delegated to IT departments. They are business transformations enabled by technology, and as such, they demand active and visible ownership from the top. The CEO, not just the CIO, must be the ultimate sponsor. When the C-suite presents a united front, it signals to the organization that the program is not optional, not experimental, but central to the firm’s future.

Clarity of purpose is paramount. Every transformation should be anchored in a simple, compelling “why” that ties directly to business outcomes. When difficult trade-offs arise, as they inevitably will, leaders should test each decision against the strategic rationale. Without this anchor, programs drift into technical exercises devoid of business relevance.

Executives must also embrace realism. Transformations will cost more and take longer than initial projections suggest. Leaders should resist the temptation to pack in every conceivable feature and instead enforce ruthless prioritization. A disciplined focus on a minimum viable product can deliver tangible value early, build organizational confidence, and provide real-world feedback to guide subsequent phases.

Change management must be treated as seriously as technology implementation. Too often, communication, training, and employee support are underfunded afterthoughts. In reality, they are as critical to success as the software itself. Executives should champion change at every level, empowering internal champions and fostering a culture of adaptability.

Finally, governance must be transparent and unsparing. Metrics should go beyond budget and schedule to include adoption and business value realization. Steering committees must be willing to make difficult calls, including changing direction or cancelling projects that no longer justify their investment. The sunk cost fallacy is a powerful trap, but strong leadership can resist it.

## Conclusion

The story of Lidl’s failed transformation is dramatic, but it is far from unique. Across industries and geographies, large-scale technology programs routinely falter under the weight of unrealistic expectations, weak governance, cultural resistance, and strategic misalignment. For senior executives, the message is sobering but also empowering. These failures are not inevitable. They stem less from technology than from leadership choices. By owning the transformation, anchoring it in clear business outcomes, enforcing discipline in scope and governance, and investing deeply in change management, leaders can break the pattern of failure.

The large transformation antipattern is real, but it is not destiny. For those willing to lead with clarity, courage, and discipline, technology transformation can deliver the competitive advantage it promises rather than the cautionary tale it too often becomes.

## References

BCG. (2024, November 13). _Most large-scale tech programs fail—Here’s how to succeed_. Boston Consulting Group. Retrieved from [https://www.bcg.com/publications/2024/most-large-scale-tech-programs-fail-how-to-succeed](https://www.bcg.com/publications/2024/most-large-scale-tech-programs-fail-how-to-succeed)

Bloch, M., Blumberg, S., & Laartz, J. (2012). _Delivering large-scale IT projects on time, on budget, and on value_. McKinsey & Company. Retrieved from [https://www.mckinsey.com/capabilities/digital/our-insights/delivering-large-scale-it-projects-on-time-on-budget-and-on-value](https://www.mckinsey.com/capabilities/digital/our-insights/delivering-large-scale-it-projects-on-time-on-budget-and-on-value)

Garcia, J. (2022, March 29). _Common pitfalls in transformations: A conversation with Jon Garcia_. McKinsey & Company. Retrieved from [https://www.mckinsey.com/capabilities/transformation/our-insights/common-pitfalls-in-transformations-a-conversation-with-jon-garcia](https://www.mckinsey.com/capabilities/transformation/our-insights/common-pitfalls-in-transformations-a-conversation-with-jon-garcia)

Gartner. (2019). _Tackle the Biggest Challenges of Transformation_. Gartner, Inc. Retrieved from [https://www.gartner.com/smarterwithgartner/tackle-the-biggest-challenges-of-transformation](https://www.google.com/search?q=https://www.gartner.com/smarterwithgartner/tackle-the-biggest-challenges-of-transformation)

Gross, I. (2018, July 20). _Lidl IT debacle: €500m down the drain_. E3 Magazine. Retrieved from [https://e3zine.com/lidl-it-debacle-e500m-down-the-drain/](https://www.google.com/search?q=https://e3zine.com/lidl-it-debacle-e500m-down-the-drain/)

Infosys. (2021). _Digital Transformation: Challenges and Potential Pitfalls_. Retrieved from [https://www.infosys.com/services/data-analytics/documents/challenges-potential-pitfalls.pdf](https://www.infosys.com/services/data-analytics/documents/challenges-potential-pitfalls.pdf)

McKinsey. (2020). _An interview with Harry Robinson on technology transformations_. McKinsey & Company. Retrieved from [https://www.mckinsey.com/capabilities/digital/our-insights/an-interview-with-harry-robinson-on-technology-transformations](https://www.google.com/search?q=https://www.mckinsey.com/capabilities/digital/our-insights/an-interview-with-harry-robinson-on-technology-transformations)

Taylor, R. (2021). _Avoiding the Pitfalls of Large-Scale Digital Transformations_. CGI Inc. Retrieved from [https://www.cgi.com/sites/default/files/2021-06/avoiding\_the\_pitfalls\_of\_large\_scale\_digital\_transformation.pdf](https://www.cgi.com/sites/default/files/2021-06/avoiding_the_pitfalls_of_large_scale_digital_transformation.pdf)

Tsty, D. (2019, April 16). _Lidl’s Failed SAP Implementation: A Case Study in Why ERP Projects Fail_. ERP Focus. Retrieved from [https://www.erpfocus.com/lidl-sap-implementation-failure.html](https://www.google.com/search?q=https://www.erpfocus.com/lidl-sap-implementation-failure.html)