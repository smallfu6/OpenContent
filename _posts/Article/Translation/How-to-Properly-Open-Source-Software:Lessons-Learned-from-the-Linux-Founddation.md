
来源：https://www.youtube.com/watch?v=9wDusmibYCg

大家好，我是哈特，今天我将讨论如何开源代码。我认为这次的内容会比之前的一些演讲更务实。

但我将首先谈谈一些开源的背景，为什么我们要开源？以及关于Linux基金会的一些内容。重点是为什么你应该关注我对如何开源代码的看法，然后我将讨论一些开源的基本要素，这些是你在正确开源代码时必须掌握的。

这将包括软件许可、知识产权保护和最佳安全实践。最后，我将谈谈开放治理和开放社区，所以让我们开始吧。让我们回顾一下，为什么我们要开源代码？

主要有两个原因，第一是让其他人能够验证、检查和学习我们的代码。如果我们希望人们信任我们的工作，就必须向他们展示代码。开源还有许多关于软件安全的好处。但开源代码的主要原因可能是让其他人能够使用甚至贡献我们的代码。

在开源中合作有许多经济效率，围绕一段开源代码的大型生态系统确保即使一个组织消失，开发仍将继续。

因此，开源软件在更广泛的生态系统中取得了胜利。如果你是开发者，你可能知道这一点。但对于许多商业应用，甚至是典型的商业应用，即使是闭源的，现代应用程序的代码库中有90%是开源的。如果我们看看今天世界上软件的构建方式，甚至是商业软件，这大致就是它的样子。人们从一个开源软件框架开始，然后使用自定义代码和现有库来解决问题。

这可以带来巨大的经济效率。我知道这是一个密码朋克的主题。但如果你试图说服你的老板让你开源代码，经济效率是一个很好的论点。

但开源在多个公司、实体或个人合作构建他们都需要的软件时最有效。你可以把这看作是去中心化开发，而这正是Linux基金会所解决的问题，我们为开源代码解决去中心化开发。当多个公司、实体或个人想要在开源软件上合作，但又不信任单一方拥有代码时，他们会求助于Linux基金会。

这正是区块链人士通常会感到舒适的事情，这太棒了。因此，我不想把这变成Linux基金会的宣传片，但我确实想提供一些事实和数据。希望这些能说服你。我们拥有数据和经验，可以为开源代码提供正确的建议。我们支持一些世界上最关键的项目。可能每个人都知道Linux内核，也许你在进行云开发时使用Kubernetes。

但你可能不知道，世界上很大一部分的电信基础设施是基于Linux基金会的开源代码运行的。或者说，如果你有一辆新车，它可能运行在Linux上，可能使用类似于汽车级Linux的东西。你知道，还有一些有趣的项目，比如学院软件基金会，它托管着好莱坞用来制作动画的软件，还有像RISC-V这样的项目。

只是一些数字。我不会逐一读给你听，但希望我能让你相信，在开源方面我们见识过一切。我为什么在这里？好吧，我们在以太坊领域也有一些项目。这里的许多人可能知道Basu，它是以太坊核心执行客户端之一。

我们在开源生态系统中还有许多其他以太坊工具，比如Web3J，你可能用它来开发以太坊。还有Paladin，这是一个全新的EVM隐私实验室。再说一次，所有这些代码库都是完全免费和开放的，所以如果你想，今天就可以去使用。

好的，让我们进入演讲的核心内容。我们来谈谈开源软件。基本要求。你需要做些什么来确保你在开源代码时有良好的体验？我们来看看开源软件的定义，对吧？

这是一种软件，其源代码是在许可证下发布的，关键字是许可证。显然，在这种情况下，许可证是一个法律文件，表达了与代码相关的权利和责任。

所以我们今天看到的开源许可证主要有三种典型类型。我们有商业许可证，这通常是非常限制性的软件许可证，可能需要向开发公司支付使用费用。我们有版权归属许可证，比如GPL许可证，修改软件时需要你回馈任何衍生作品或在软件基础上构建的内容。最后，我们有宽松许可证，这让你可以以任何方式使用和修改软件。我将详细介绍这些许可证。

那么我们先从BSL许可证开始，技术上来说，商业源许可证并不是开源许可证，而是一种源代码可用许可证。源代码是公开的，但只有在满足某些条件时，你才能使用这些源代码。这被视为专有软件和开源软件之间的一种妥协。

如果你想获得人们看到和信任你的代码的一些好处，但又希望人们为此付费，这就是人们通常会做的。

BUSL就是一个例子，在以太坊领域，Arbitrum和Nitro使用了这种许可证。现在我们来谈谈版权归属许可证，这些是要求用户提供所有衍生作品的开源许可证。因此，如果你修改代码并在某个项目中使用，通常需要将其源代码免费提供，并且也要在这个版权归属许可证下授权。

版权归属许可证在商业使用中往往非常困难。著名的例子有MPL、GPL和LGPL，在以太坊社区中，Geth就是一个显着的例子。

所以我引用理查德·斯托曼关于GNU和反版权许可证的话，并对反版权许可证发出警告。反版权许可证的目标是通过法律要求来增加贡献。而这些许可证的不幸现实是，人们根本不会使用你的代码。如果由于潜在繁琐的法律要求存在任何可行的替代方案。我想说，从反版权许可证转为宽松许可证是非常困难的，所以请谨慎选择。

最后，还有宽松许可证，这些是允许你自由修改和使用代码的开源许可证。

目前，大多数商业使用的开源代码都使用宽松许可证，因为它们是最容易使用的。如果你想最大化社区对你代码的采用，我们强烈建议你使用宽松许可证。你可能见过Apache 2和MIT作为例子。在以太坊领域，有很多项目，Basu就有一个Apache许可证。在我们进一步讨论之前，我想提到一些常见的许可证陷阱。

你知道，我在这个会议上与大多数人谈过，看到人们犯这些错误。所以我想谈的是对你使用的代码要非常小心，对吧？这有点像LGPL依赖问题。当你使用包含LGPL代码的组合作品时，这意味着你将LGPL代码放入更大的项目中。有时人们认为如果它在一个单独的文件夹中，就可以链接。

但正如这一条款所示，你不能对LGPL代码有编译时依赖，它必须是运行时依赖，所以请仔细检查你的依赖。

最后，要小心没有知识产权保护的许可证。这是来自一个匿名公司文档的例子。基本上说，我们将对代码使用宽松许可证，但我们会对这段代码执行专利。因此，使用这段代码仍然需要付费。请仔细阅读。这家公司实际上非常透明。

如果你使用来自不太道德和透明的人的代码，你可能会面临诉讼的风险。总之，我要说的是，密切关注你使用的开源项目的许可证和许可要求。我个人推荐你为自己的代码使用Apache 2，因为它是一个宽松许可证，并且有明确的专利授权保护。如果你想让一个专有代码库对他人可见，可以考虑使用BSL许可证，对吗？

现在我们继续。我们一直在谈论知识产权保护，那么当你需要保护你的代码免受知识产权问题时该怎么办呢？有时，贡献者可能无意中或恶意地向你的项目添加一些具有某种知识产权保护的代码。结果是，我们在Linux方面遇到了一个大问题。

有人知道SCO与Linux的争议吗？

是的，有些人知道。这是大量的诉讼。基本上是因为内核没有明确的知识产权保护。为此，LF的人员创建了开发者来源证书，我们建议你为你的代码使用开发者来源证书或贡献者许可证协议。围绕你的代码建立这些法律框架非常重要。

如果你接受外部贡献，这一点尤其重要。

所以，举个例子，这就是DCO，就这样。使用带有Dash S标志的签名提交在GitHub上设置非常简单。刚开始可能需要一点适应。

但一旦你的贡献者习惯了，这就非常简单，对吧？总之，确保你的代码有法律保护。如果没有，可能会被起诉的人会非常犹豫使用你的代码。我们实际上要求所有Linux基金会项目都必须有这种保护。

如果你贡献代码，你必须有这种保护，你也应该有。对于你的开源软件，我们使用DCO。但再次强调，CLA也是完全可以接受的。

好的，那么安全性怎么样？显然，安全性对任何软件都是至关重要的，不仅仅是开源软件。我们可以专门举办一个关于开源安全的会议。实际上，上个月就有一个。

但我想简要强调一些可能与开源不同的内容，包括漏洞披露、SBOM（软件账单和材料）以及软件认证。所以我想说，我们在Linux基金会有一个很棒的组织，叫做OpenSSF，提供所有开源软件的最佳实践。如果你对安全有任何问题，可以去看看。

这是一个很好的资源，可以确保你做的每件事都是正确的。那么安全性、漏洞披露和管道呢？开源软件的一个明显优势是社区成员可以发现并报告错误。关键是，你希望尽可能让他们做到这一点，对吧？

你不希望贡献者之间出现摩擦。这并不在乎你设置的具体方法，只要它易于遵循即可。我想说，在LF中，我们的许多项目使用了GitHub工具，但并不是所有项目都这样。例如，Basu有七个报告渠道，这对我们来说可能是一个挑战。

但我们现在确实如此，继续前进，回想一下我说过，现代软件是这样构建的，对吧？

这非常好且高效，但也引入了一些问题。如果你在有安全漏洞的软件上构建，可能会遇到真正的问题。事实证明，最近许多被公开的大规模攻击和造成的诸多问题，都是由于这些所谓的软件供应链攻击。而阻止这些攻击的解决方案通常被称为软件材料清单，或SBOM。这里的每个人都听说过SBOM吗？

有些人听说过，太好了。如果你没有听说过，绝对应该了解一下。SBOM让你能够跟踪你在开源软件项目中引入的所有代码。

如果有漏洞，你可以快速找到并更新它们，对吧？我还鼓励你仔细检查你使用的代码，以确保它得到良好维护。不要引入来自某个四年前没有更新的随机开发者的代码。

我再说一遍。管理良好的开源项目对所使用的依赖非常谨慎，并且有很多优秀的工具可以帮助实现这一点。GUAC非常出色，但还有许多其他工具，对吧？所以我将简要谈谈软件和工件认证。

如果你在一个受欢迎的开源项目中进行开发，人们会试图冒充你。这种情况在我们LF经常发生，你知道，就在上个月，有人创建了一堆假冒的NPM包来试图冒充我们。但是，你知道，有很多工具可以用来签名和验证代码。我认为第六道门是一个很好的例子。

不过我确实希望并认为它们应该在区块链上运行。

好的，我们已经讨论了一些基本内容。那么，建立一个开放社区呢？如果我们回到开源软件的定义，这里有一个关键点是“协作、公开的方式”这个短语。这很重要，因为特别是宽松许可证所提供的自由，允许大型和多样化的社区围绕流行软件形成，对吧？

这使得开源的经济效率得以实现。所以当我们谈论开放开发和开放协作时，我们不仅仅是指开源，对吧？我们还指开放开发。这意味着有一个社区在公开的环境中积极构建开源代码，以及开放治理，这意味着社区的程序和角色，项目和路线图的决策和优先级是公开定义和管理的。所以我将介绍一些开源治理模型，这是一种连续体。

这并不是说只有这四种形式，只是给你一个关于如何设置开源项目的感觉。所以最不开放的形式被称为我喜欢称之为公共演示，代码只是开源的。它就在那里。

这并没有真正更新，也不一定有路线图。你可以不那么客气地称之为代码倾倒。

接下来我们就进入开放公司产品的阶段，对吧？这指的是公司或实体将一款软件开源，成为一个产品，对吧？它不允许外部贡献，或者使其非常困难，但它保持路线图，定期发布，并遵循最佳安全实践。随着我们变得更加开放，我们有了仁慈独裁者项目。这是指一个组织或个人开源他们的代码，并允许外部贡献者的贡献。

但项目的最终权威仍然是那个仁慈的组织。最后，我们有真正的开放治理，这意味着代码有透明的文档，去中心化的，基于优点的治理，托管在一个中立的实体下。任何人都可以加入。领导层有包容性和明确的流程，没有限制谁可以加入并成为领导者。对吧？所以我们可以更详细地讨论这些代码模型，对吧？

我确实相信，公开演示代码比根本不开放代码要好，对吧？第三方可以审计你的代码，看看你在做什么，人们会信任你。我们从大公司那里得到的最大反对意见是存在声誉风险。我的回应通常是，如果你试图构建一个生产系统，就不应该为让别人看到你的代码而感到尴尬。

如果是那样，那就是个问题。

你知道，一旦我们转向一个更开放的产品，这可能比公开演示要容易一些。但要让其他人使用你的代码仍然很困难，因为这个模型需要对公司有很高的信任度。如果公司改变方向，放弃软件或倒闭，那对你和你的业务可能会造成问题，尤其是当你依赖这段代码时。

然后是一种仁慈独裁者的模式，对吧？这在开放性上有所增加，但这仍然意味着你所在领域的竞争对手，或者那些不信任你的公司或实体的人不太可能参与。因此，获得贡献和让人们参与比单纯的开放产品要容易。因为人们通常可以进行小的改动，修复错误。

他们可以解决自己的痛点，但最终这并不是开放治理，最后我们有完全开放治理的项目，对吧？这强烈激励公司或其他实体或个人进行贡献，因为他们可以根据自己的贡献在治理中发挥作用，拥有多样化的贡献者。这意味着潜在用户可以很容易地相信项目的长期稳定性和可行性，这将增加项目的整体使用。

而这主要的缺点是这是一个社区项目，现在不再只是你的项目。参与的人应该根据他们的贡献获得相应的治理权，对吧？

关于治理，我鼓励你仔细选择要使用或参与的项目，基于社区所采用的治理风格。无论你选择什么治理方式，确保清晰地记录下来。如果你的主要目标是发展社区，我们强烈推荐开放治理的项目。正如你所知，我们在过去的两分钟里讨论过这个，对吧？最后，我想谈谈一些发展社区的最佳实践。

一个最佳实践是开放源代码的二元治理，这就是我之前提到过的，虽然我没有真正称之为这个。那些经受住时间考验的最成功项目拥有中立、开放的治理模式，做事的人做决定。再说一次，这并不是很赛博朋克，但它们是最持久、最成功的。开放源代码产品也有良好的商业支持生态系统，以及多样化的商业支持生态系统。

因为那些从代码中赚钱的人可以将其投入到代码的贡献中。吸引潜在竞争者的投资是困难的。如果一个实体拥有或控制代码库，我们建议建立一个中立的环境或在代码库周围建立某种中立性。最后，拥有透明、记录清晰的治理非常重要。因此，想要参与的人会想确切知道他们如何参与，他们不想感到意外，对吧？

这似乎很难。我该怎么办？好吧，看看Linux基金会或其他开源软件基金会。你知道的，像Apache软件基金会这样的组织。作为一个家，LF的角色再次是作为一个中立的组织来托管代码。如果你没有这个或需要这个，我们可以提供帮助。

你知道，我们几乎得到了所有大科技公司的信任。建立一个开源社区是很困难的。我们在这方面有经验，和我们以及其他软件基金会一样，法律结构至少对我们来说可以保护内核，Kubernetes也可以保护你的项目。最后，我想强调的是，贡献代码或项目对任何人来说都是完全免费和开放的。

所以，任何Linux基金会的项目你都可以加入，你可以使用代码，也可以贡献代码，都是免费的，完全开放的。如果你有任何问题，欢迎在Linux基金会去中心化信任找到我们，非常感谢你的时间。

好的，再次感谢你，Hart。我们这里有几个问题。你能解释一下MIT和Apache 2.0许可证之间的区别吗？好问题。

这是一个难题，真正的答案甚至可能在法律上也不明确。因为我们没有法院案例来区分这些许可证。再次声明，我不是律师，这不是法律建议。主要区别在于Apache 2.0许可证有明确的专利保护，这种情况尚未发生。但可能会出现对MIT代码库成功的专利诉讼，而对Apache 2代码库则没有。

目前，这种情况并不存在，你知道吗？现在，它们大致相同，都是兼容的许可证，你可以互换使用。但是，如果你特别谨慎，可能会想使用Apache 2.0，对吧？

确保开源项目财务可持续性的最有效收入策略是什么？如何建立足够的社区兴趣以实现这种可持续性？这是个很好的问题。我们可以为此进行一次完整的讨论。这真的取决于你的商业模式。有许多成功的开源商业模式。

我相信在场的许多人都有这样的经验。但关键是，人们应该在商业中成功使用开源软件，对吧？无论是基于开源模型提供服务，这是一种非常流行的方式，还是在开源模型上销售高级产品或软件。

这大致是两种主要模型，还有很多其他模型，但关键是围绕此建立商业生态系统。如果我知道每种应用的答案，我就会成为亿万富翁的软件高管，但我不是。

所以，我想这确实取决于项目。也许在另一个人生中。好吧，接下来的问题，精彩的演讲。但我们如何让普通人真正关心开源软件呢？

这是个很好的问题。我们在Linux基金会总是在努力做到这一点。我认为与开发者的对话要容易得多。

所以，我不知道，我对这个问题没有一个好的答案。我认为这是一个困难的问题。人们首先需要理解软件和软件开发。

所以这是个难题。下一个问题是，你谈了很多关于治理的内容。链上治理能帮上忙吗？从长远来看，链上治理可能会有所帮助。你知道，现在律师们非常不安，先例实际上还没有建立。

你知道，我对长远的未来持乐观态度，认为我们至少可以在链上实现一些治理。是的，没错。在一个人们拥有更好法律框架或更少无谓法律斗争的世界里，你希望有多少最佳实践不再需要？我当然希望我们有一个不那么疯狂的软件专利系统，这样我们就不必不断参与相互确保毁灭的专利行为。

所以，我希望看到这一点得到改善。你知道，有些许可是，企业确实需要从开源软件中获利。但我确实认为专利系统是一团糟。

我怎么能确定呢？是的。你如何设想开源软件在一个越来越依赖去中心化和隐私保护解决方案的世界中演变？你知道，去中心化的解决方案本质上意味着更多的人需要聚集在一起解决问题，对吧？

这将意味着开源将扮演更重要的角色，因为你知道，人们共同构建软件的唯一有效方式，实际上是在一个中立的环境中，对吧？我们必须为软件建立去中心化的中立环境。所以我认为去中心化技术将真正加速开源的发展和使用。我们在银行业已经看到了很多这一点。

好的，有什么资源可以帮助从仁慈的独裁转向开放治理模式吗？当然，我们在Linux基金会有很多这样的资源，你可以去看看我们的网站。

来和我们谈谈。这是一个非常常见的问题，我们经常被问到，我们在这方面有很多经验。

好的，最后一个问题，LF是否关注公共利益资金实验？在以太坊生态系统中？我们定期关注资金问题。你知道，我们是一个非营利组织，所以我们没有很多钱可以分配。
