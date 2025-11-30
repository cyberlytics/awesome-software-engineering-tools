[//]: # (Author: Christoph P. Neumann)
[//]: # (Title: Awesome Software-Engineering: Tools)
[//]: # (Language: de-DE)
[//]: # (Licence: CC BY 4.0)
[//]: # (Kurztitel: Werkzeuge » SWE)
[//]: # (Lemma: tools-swe)

# Awesome Software-Engineering: Tools

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Made With Love](https://img.shields.io/badge/Made%20With-Love-pink.svg)](https://github.com/chetanraj/awesome-github-badges)
[![Donate via PayPal](https://img.shields.io/badge/Donate-PayPal-blue?logo=paypal)](https://www.paypal.com/donate/?hosted_button_id=QTDJ2JA58ZM9L)
[![Support on Ko‑fi](https://img.shields.io/badge/Donate-ko--fi-%23FF5E5B?logo=ko-fi&logoColor=white)](https://ko-fi.com/cyberlytics)
[![Buy Me A Coffee!](https://img.shields.io/badge/Donate-buymeacoffee-%23FFDD00?logo=buymeacoffee)](https://www.buymeacoffee.com/cyberpetaneuron)

Es gibt von mir die weiteren Schwesterseiten im Kontext Informatik/KI: [Digitaler Ressourcen-Pool](https://github.com/cyberlytics/awesome-basics), [Werkzeuge » Abschlussarbeiten](https://github.com/cyberlytics/awesome-thesis-tools) und [Werkzeuge » BDCC/AI](https://github.com/cyberlytics/awesome-bdccai-tools).

Hinweise:

- Die Werkzeuge sind im Zweifelsfall für Studierende und private Nutzung, weniger für Unternehmen oder Freelancer (wegen der Lizenzbedingungen/EULA)
- Entstanden an der [OTH Amberg-Weiden](https://www.oth-aw.de/cpn), welche für ein paar Einträge entsprechend den Kontext bildet.
- Die kostenlosen Werkzeuge sind nicht immer Best-in-Class im Vergleich zu kostenpflichtigen/„(€)“ Alternativen, dennoch bleiben kostenpflichtige Angebote hier meist Out-of-Scope
- Ein Windows-zentrischer Ersteindruck durch die Chocolatey-Referenzen kann leicht täuschen, denn die kostenlosen oder quelloffenen Tools gibt es i.d.R. auch für Linux oder macOS mittels snap/flatpak/brew/etc.
- Empfehlung zu [Chocolatey](https://chocolatey.org/install): **choco feature enable -n useRememberedArgumentsForUpgrades**

**Table of Contents**

<!-- toc -->

- [git](#git)
- [Programmierung](#programmierung)
- [Rapid Application Development](#rapid-application-development)
- [Vibe Coding](#vibe-coding)
- [SW-Bibliotheken & -Frameworks](#sw-bibliotheken---frameworks)
- [Testing](#testing)
- [Fehleranalyse](#fehleranalyse)
- [Wireframing & Prototyping & UX](#wireframing--prototyping--ux)
- [Modellierung & Architektur](#modellierung--architektur)
- [DevOps](#devops)
- [Software-Internationalisierung (I18n) & -Lokalisierung (L10n)](#software-internationalisierung-i18n---lokalisierung-l10n)
- [Quantencomputing](#quantencomputing)
- [Kostenlose Alternativen](#kostenlose-alternativen)
- [Bonus: Studentisches Start-Up (Software-Entwicklung)](#bonus-studentisches-start-up-software-entwicklung)
- [Appendix: App Recommendations & Repos](#appendix-app-recommendations--repos)
- [Appendix: More Free Student Stuff](#appendix-more-free-student-stuff)
- [Footer](#footer)
  - [Future Work](#future-work)
  - [Contribute](#contribute)
  - [Backers](#backers)
  - [License](#license)

<!-- tocstop -->

## git

- Git Client: **[git](https://gitforwindows.org/)** \[**choco install git.install -y --params="'/GitAndUnixToolsOnPath /WindowsTerminal /NoAutoCrlf'"**\]
	- ggf. **[TortoiseGit](https://tortoisegit.org/)** \[**choco install tortoisegit**\] | [SourceTree](https://www.sourcetreeapp.com/) \[choco install sourcetree\] | [SmartGit](https://www.syntevo.com/smartgit/) \[choco install smartgit\] | [GitKraken](https://www.gitkraken.com/GitHub-student-developer-pack-bundle) (s. unten)
- Git Server:
	- **[Gogs](https://gogs.io/)** \[**choco install gogs**\]: painless self-hosted Git service in go
	- Weitere Alternativen per Linux oder Docker: [Forgejo](https://forgejo.org/) (community-governed fork of [Gitea](https://about.gitea.com/)) sowie [GitLab CE](https://gitlab.com/gitlab-org/gitlab-environment-toolkit)
- **[GitHub CLI](https://cli.github.com/)** \[**choco install gh**\]: gh is GitHub on the command line, it brings pull requests, issues, and other GitHub concepts to the terminal ([gh-Cheatsheet](https://www.kdnuggets.com/2023/03/GitHub-cli-data-science-cheat-sheet.html))
- Utilities:
	- **[git-sizer](https://github.com/GitHub/git-sizer)** \[**choco install git-sizer --ignore-dependencies**\]
	- git-Graphen zeichnen: [Mermaid Gitgraph Diagrams](https://mermaid.js.org/syntax/gitgraph.html)
	- Fortgeschrittene Git-Repo-Analysen: **[Hercules](https://github.com/src-d/hercules)**
	- Animierte Visualisierung der Git-Repo-Historie: **[gource](https://gource.io/)**
- **[GitHub Education](https://education.github.com/benefits?type=student)**: insbesondere [GitHub Pro](https://docs.github.com/en/get-started/learning-about-GitHub/GitHubs-products#GitHub-pro) ist dadurch für Studierende kostenlos
- **[GitKraken Client Pro](https://www.gitkraken.com/GitHub-student-developer-pack-bundle)** [und](https://www.gitkraken.com/GitHub-student-developer-pack-bundle) **[GitLens+ Pro](https://www.gitkraken.com/GitHub-student-developer-pack-bundle)** sind für Studierende kostenlos
- **[gitattributes](https://richienb.github.io/gitattributes-generator/)**-Generator (Obacht: LF-formatiert) von Richie Bendall
- **[gitignore](https://www.toptal.com/developers/gitignore/)**-Generator (Obacht: LF-formatiert) von Toptal
- **[wget](https://www.gnu.org/software/wget/)** \[**choco install wget**\]: im Kontext von git u.a. für: **wget -O LICENSE "[https://www.apache.org/licenses/LICENSE-2.0.txt](https://www.apache.org/licenses/LICENSE-2.0.txt)"** (Obacht: LF-formatiert)
- **[eolConverter](https://github.com/jurosh/nodejs-eol-converter-cli)** \[**npm i -g eol-converter-cli**\]: Unter Windows benötigen Sie u.a. für das Repo-RampUp meist ein Werkzeug für EOL-Konvertierungen, u.a. für:
	- Ramp-Up: eolConverter **crlf "\*\*/.gitattributes"** | eolConverter **crlf "\*\*/.gitignore"** | eolConverter **crlf "\*\*/LICENSE"**
	- Sporadisch: eolConverter **crlf "src/\*\*/\*.{txt,js,java,svg}"**
- gitlog-Hygiene hinsichtlich Autorenliste:
	- A priori: **git config** --global **user.name** "Erika Musterfrau" | **git config** --global **user.email** [e.musterfrau@oth-aw.de](mailto:e.musterfrau@oth-aw.de)
	- A posterio: Überprüfen Sie mittels „**git shortlog -se**“ Ihre Autorenliste und denken Sie über eine **[.mailmap](https://git-scm.com/docs/gitmailmap)** in Ihrem Repo nach
- git-**Hygiene** (#1) hinsichlich Security Credentials (und übergroßer Dateien):
	- Secrets Scanning (CLI): **[TruffleHog](https://github.com/trufflesecurity/trufflehog)** \[**choco install trufflehog**\], **[Gitleaks](https://github.com/gitleaks/gitleaks)** \[**choco install gitleaks**\]
	- Secrets Scanning (Cloud): **[GitGuardian](https://www.gitguardian.com/)**
	- Cleaner (CLI): [**BFG** Repo-Cleaner](https://rtyley.GitHub.io/bfg-repo-cleaner/) (zzgl. Ramy McCarthys Artikel [Removing sensitive data from a Github repository](https://ramimac.me/2022/07/31/Github-Cleanup/))
- git-**Hygiene** (#2) hinsichtlich Autoren (insb. Eliminierung privater Mail-Adressen und Konsolidierung von Autorennamen):
	- Mit einer manuell erstellten **[.mailmap](https://git-scm.com/docs/gitmailmap)** und dem Skript **[git-filter-repo](https://github.com/newren/git-filter-repo/blob/main/git-filter-repo)** können Sie die Autoren auch hart umschreiben
- **[Gravatar](https://de.gravatar.com/)**: Viele git-Analysewerkzeuge greifen auf Gravatare zurück
- LLM-generated Commit Messages:
	- [gitprompt](https://github.com/xyassini/gitprompt)
- git repo README embeddings:
	- [RepoGraphy](https://repography.com/): Graphical Dashboard mit Git-Repo-Metriken
	- githum.com [Star History](https://www.star-history.com/#cyberlytics/awesome-basics&Date)
- Weiterführende Quellen: [Awesome git](https://github.com/dictcp/awesome-git)

## Programmierung

- Code Qualität Selbstcheck? **Statischer Code Analyzer** ⚠️ bzw. Linter, wie bspw. **[PMD](https://pmd.GitHub.io/)**
	- **Keine Copy-Paste-Programming** ⚠️, bspw. per **[CPD](https://pmd.GitHub.io/latest/pmd_userdocs_cpd.html)** überprüft, welcher in der Installation von PMD enthalten ist
	- Alternativen: [NetAnalyzers](https://learn.microsoft.com/de-de/visualstudio/code-quality/install-net-analyzers) (C#), [ESlint](https://eslint.org/) (JS), [CSS Lint](http://csslint.net/) (CSS), [perlcritic](https://metacpan.org/dist/Perl-Critic/view/bin/perlcritic) (Perl), etc. pp.
	- Weiterführende Quellen: **[Awesome Static Analysis](https://github.com/awesome-security/awesome-static-analysis)** | Awesome **[Static Analysis](https://github.com/analysis-tools-dev/static-analysis)** + **[Dynamic Analysis](https://github.com/analysis-tools-dev/dynamic-analysis)**
- Coding Conventions Selbstcheck? **Code Style Checker** ⚠️ wie [checkstyle](https://checkstyle.sourceforge.io/) (Java), [StyleCop](https://github.com/DotNetAnalyzers/StyleCopAnalyzers) (C#), [JSCS](https://jscs-dev.GitHub.io/) (JS), etc. pp.
	- Zzgl. **Auto-Formatter** ⚠️, welche in den meisten IDEs eingebaut sind, meist per **Ctrl+Shift+F**
	- Zzgl. **Code-Cleanup** ⚠️ Funktionalitäten, bspw. [Eclipse's Clean Up](https://help.eclipse.org/latest/index.jsp?topic=%2Forg.eclipse.jdt.doc.user%2Freference%2Fpreferences%2Fjava%2Fcodestyle%2Fref-preferences-cleanup.htm) bzw. [Intellij IDEA's Code Cleanup](https://www.jetbrains.com/help/idea/reformat-and-rearrange-code.html) (Java) oder [ReSharper’s Cleanup Code](https://www.jetbrains.com/help/resharper/Code_Cleanup__Index.html) (C#)
- SQL:
	- IDE? **[DataGrip](https://www.jetbrains.com/datagrip/)** (siehe unten)
	- SQL-Dialekt-Konvertierung: [SQLines](https://www.sqlines.com/online)
	- SQL-Testing: siehe unten
	- KI-gestützte SQL Code-Completion: siehe unten
	- E/R-Diagramme: siehe unten
	- Schema Diagrams: siehe unten
- [Visual Studio **Code**](https://code.visualstudio.com/) \[**choco install vscode --ignore-dependencies**\]
	- Es gibt viele wertvolle Extensions → [Awesome VS Code](https://github.com/viatsko/awesome-vscode) bzw. [Best-Of-Listen](https://metager.org/meta/meta.ger3?eingabe=best+vs+code+extensions)
	- Auswahl: [PlantUML](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml), [draw.io](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio), [AsciiDoc](https://marketplace.visualstudio.com/items?itemName=asciidoctor.asciidoctor-vscode), [SonarLint](https://marketplace.visualstudio.com/items?itemName=SonarSource.sonarlint-vscode), [TabNine](https://www.tabnine.com/install/vscode), uvm.
	- Mit Student-Subscriptions (s. unten): [GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot), [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- Kollaboratives Programmieren? (Coding Dojos | Job Interviews) ⊂ DEVaaS
	- **Ohne Registrierung**
		- Cloud (any lang): **[Collabedit](http://collabedit.com/)** (aber leider keine Code-Ausführung 😞)
		- Cloud (JS-only): **[JSFiddle](https://jsfiddle.net/)** (mit Code-Ausführung 😃; auch kompatibel zu einer einfachen Jasmine-via-Browser Konfiguration, wie in PK3 verwendet)
	- Mit Registrierung
		- Cloud: **[neverinstall](https://neverinstall.com/spaces/devtools)** (free: 2 Users, max. 1 hour screen time) und **[GitPod](https://www.gitpod.io/pricing)** SaaS (free: 50 hours/month)
		- On-Premise: **[GitPod](https://www.gitpod.io/)** Self-Hosted Community License (free: ≤10 users)
- DEVaaS (Single User Perspektive):
	- Programmierumgebungen (diverse Programmiersprachen) in der Cloud? **[neverinstall](https://neverinstall.com/spaces/devtools)**, **[GitPod](https://www.gitpod.io/)**, **[Geeks-for-Geeks IDE](https://ide.geeksforgeeks.org/)**, uvm.
	- Py-only: **[python anywhere](https://eu.pythonanywhere.com/pricing/)** (kostenlose Browser-basierte Python-WebApp-Umgebung)
	- JS-only: **[CodeSandbox](https://codesandbox.io)**, **[StackBlitz](https://stackblitz.com)**, **[PlayCode](https://playcode.io/)**, [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/), [Plunker](https://plnkr.co/), [JDoodle](https://www.jdoodle.com/html-css-javascript-online-editor/), uvm.
	- Java-only: [**JDoodle** Advanced](https://www.jdoodle.com/online-java-compiler-ide/) ([Basic](https://www.jdoodle.com/)) , tutorialspoint **[Online Java Compiler](https://www.tutorialspoint.com/compile_java_online.php)**
- **JetBrains**: Bspw. für **[PyCharm](https://www.jetbrains.com/pycharm/)** (Py), **[WebStorm](https://www.jetbrains.com/webstorm/)** (JS), **[CLion](https://www.jetbrains.com/clion/)** (C/C++), [Intellij **IDEA**](https://www.jetbrains.com/idea/) (Java, [Kotlin](https://github.com/JetBrains/kotlin)), **[ReSharper](https://www.jetbrains.com/resharper/)** (C#) / **[Rider](https://www.jetbrains.com/rider/)** (C#) sowie **[DataGrip](https://www.jetbrains.com/datagrip/)** (SQL), uvm.
	- Kostenlos über die [Free Educational Licenses](https://www.jetbrains.com/community/education/#students) für Studierende.
	- (Unter Windows bspw. mittels chocolatey: **choco install jetbrainstoolbox**)
	- Das Google-offizielle **[Android Studio](https://developer.android.com/studio)** \[**choco install androidstudio**\] basiert auf JetBrains Intellij IDEA
- FOSS **IDEs:**
	- Py: [Visual Studio **Code**](https://code.visualstudio.com/) \[**choco install vscode --ignore-dependencies**\], [Eric](https://eric-ide.python-projects.org/eric-download.html), [Pyzo](https://pyzo.org/start.html) \[**choco install pyzo.install**\], [Kate](https://kate-editor.org/de/get-it/), [Thonny](https://github.com/thonny/thonny/releases), [PyDev](https://www.pydev.org/) \[**choco install pydev**\], [Spyder](https://www.spyder-ide.org/)
	- Java: **[Eclipse IDE](https://www.eclipse.org/downloads/packages/installer)** \[**choco install eclipse**\]
	- C#: [Visual Studio **Code**](https://code.visualstudio.com/) \[**choco install vscode --ignore-dependencies**\]
	- JavaScript: [Visual Studio **Code**](https://code.visualstudio.com/) \[**choco install vscode --ignore-dependencies**\], **[Brackets](https://brackets.io/)** \[choco install brackets\] (Nennenswert, aber tot: [Atom](http://atom.io/))
	- C/C++: **[Code::Blocks](https://www.codeblocks.org/)** \[**choco install codeblocks**\], [**Eclipse** IDE for **C/C++** Developers](https://www.eclipse.org/downloads/packages/) \[**choco install eclipse-cpp**\]
	- R: **[RStudio](https://posit.co/download/rstudio-desktop/)** \[**choco install r.studio**\]
	- PHP: **[Komodo IDE](https://www.activestate.com/products/komodo-ide/)** \[choco install komodo-ide\], [**Eclipse** PHP Development Tools (**PDT**)](https://www.eclipse.org/pdt/)
- **Microsoft Azure Dev Tools for Teaching**: Lesen Sie sich auf der [RZ-Seite „Downloads“](https://www.oth-aw.de/hochschule/services/online-services/downloads-software/) das Registrierungsverfahren und die Liste der enthaltenen Microsoft Produkte durch
- **[Swagger UI](https://swagger.io/tools/swagger-ui/)**: Für den Entwurf und die Dokumentation von REST-APIs
	- (Unter Windows bspw. mittels docker: **docker run -p 80:8080 swaggerapi/swagger-ui**)
- **[quicktype](https://quicktype.io/)**: Generate models and serializers from JSON, JSON schema, and GraphQL for any programming language
- **[Compiler Explorer](https://godbolt.org)**: interactive compiler exploration
- Weiterführende Quellen
	- Programmier-Werkzeuge: **[free-for.dev](https://free-for.dev/)** | **[The Book of Secret Knowledge](https://github.com/trimstray/the-book-of-secret-knowledge)**
	- Schauen Sie sich auch die Liste namens **[GitHub Student Developer Pack](https://education.github.com/pack)** an; das ist quasi auch eine Awesome-Liste aus Studierenden-Sicht, mit kuratierten Angeboten von GitHub-Partnern (allerdings überwiegend auf 6m oder 1a limitiert, solche Angebote halte ich für Studierende uninteressant)
	- Integrated Development Environments: [Awesome IDEs](https://github.com/zeelsheladiya/Awesome-IDEs)

## Rapid Application Development

\[ = RAD, eine Vor-Form von [Low-Code](https://github.com/cyberlytics/awesome-bdccai-tools#low-code--no-code) \]

- RAD-Tools:
	- Delphi: Embarcadero IDE namens [RAD Studio](https://www.embarcadero.com/products/rad-studio) = Der „Urvater“ moderner RAD-Tools, lebt bis heute!
	- Java: [RAPIDclipse](https://rapidclipse.com/) = Low-Code Visual Java IDE auf Basis von Eclipse (von einem Unternehmen in Weiden i.d.OPf.)
	- Python: [Anvil](https://anvil.works/) = Build seriously powerful web apps with all the flexibility of Python
	- C++: [Ultimate++](https://www.ultimatepp.org/) aka U++ = reduce the code complexity of typical desktop applications
	- Go: [pagoda](https://github.com/mikestefanello/pagoda) = Rapid, easy full-stack web development starter kit in Go
	- Rust: [Slint](https://slint.dev/)
- RAD-Programmiersprachen:
	- [dBase](https://www.dbase.com/) über xBase bis hin zu [Harbour](https://harbour.github.io/)
	- Microsoft [Visual FoxPro](http://msdn.microsoft.com/vfoxpro)
	- Weitere: [FileMaker](https://www.claris.com/filemaker/), [4D](https://us.4d.com/why-4d), ..., [Ercatons](https://www.living-pages.de/ercato/)
- Open-source RAD-Webplattformen:
	- [Appsmith](https://www.appsmith.com/)
	- [Budibase](https://budibase.com/)
	- [Foundation](https://get.foundation/)
- Microsoft RAD-Tools:
	- Microsoft [Access](https://www.microsoft.com/access)
	- Microsoft [Power Apps](https://www.microsoft.com/power-platform/products/power-apps)
	- Ice Tea Group LLC [Wisej.NET](https://wisej.com/)
- Oracle RAD-Tool:
	- Oracle [APEX](https://apex.oracle.com/)
- SAP RAD-Tool:
	- Appeon [PowerBuilder](https://www.appeon.com/products/powerbuilder)
- Rapid Prototyping (Design & UX/UI):
	- vgl. [eigener obiger Abschnitt](#wireframing--prototyping--ux)
	- zzgl. [Graphical User Interface Builder](https://en.wikipedia.org/wiki/Graphical_user_interface_builder) (aka GUI designer aka RAD IDE)
- Low Code: vgl. [Schwesterseite](https://github.com/cyberlytics/awesome-bdccai-tools#low-code--no-code)

## Vibe Coding

\[OBACHT #1: Gilt für eine Abschlussarbeit als High-Tech-Plagiarism\]
\[OBACHT #2: "Where 2 engineers can now create the tech debt of at least 50 engineers"\]

- Übersicht/Einstieg: indiehackers [Vibe Coding Tools](https://www.indiehackers.com/vibe-coding-tools) ([free ones](https://www.indiehackers.com/vibe-coding-tools?tags=Free))
- Wegbereiter:
	- Begriff: [Andrej Karpathy](https://x.com/karpathy/status/1886192184808149383) in February 2025
	- Technik: "[Cursor](https://www.cursor.com/) [Composer](https://cursor101.com/article/cursor-composer) (i.e., multi-file editing), backed with Claude [Sonnet](https://www.anthropic.com/claude/sonnet) (i.a., due to its large context window of 200K+), talked to via [SuperWhisper](https://superwhisper.com/)"
- Vibe Coding via Agentic AI (Full-Stack-Engineering Assistants)
	- Marktführer CLIs: 
		- Anthropic **[Claude Code CLI](https://docs.anthropic.com/en/docs/claude-code/overview)** \[**npm install -g @anthropic-ai/claude-code**\]
		- OpenAI [Codex CLI](https://openai.com/codex/) \[**npm i -g @openai/codex**\]
		- Google [Gemini CLI](https://github.com/google-gemini/gemini-cli) \[**npm install -g @google/gemini-cli**\]
		- GitHub [Copilot CLI](https://github.com/github/copilot-cli) \[**npm install -g @github/copilot**\]
	- Open Source CLIs:
		- [cline](https://cline.bot/) ([github](https://github.com/cline/cline)) \[**npm install -g cline**\]
			- [Roo Code](https://github.com/RooCodeInc/Roo-Code) as fork from cline
			- [Kilo Code](https://kilocode.ai/) ([github](https://github.com/Kilo-Org/kilocode)) = merged features from Roo Code and Cline plus own features
		- ollama-based CLIs:
			- [ollama code cli](https://github.com/vigyatgoel/ollama-code-cli) \[pip install ollama-code-cli\]
			- [tlm CLI](https://github.com/yusufcanb/tlm) \[irm https://raw.githubusercontent.com/yusufcanb/tlm/1.2/install.ps1 | iex\]
		- [LocalAGI](https://github.com/mudler/LocalAGI)
		- [aider](https://aider.chat/): AI pair programming \[**pip install aider-install && aider-install\]
		- [tgpt](https://github.com/aandrew-me/tgpt) (= Terminal GPT) \[**choco install tgpt**\]
	- Desktop (u.a. VS Code Extensions):
		- **[Cursor](https://www.cursor.com/)** \[**choco install cursoride**\]
		- **[Windsurf](https://windsurf.com/)** (formerly Codeium) \[**choco install windsurf**\]
		- **[TRAE IDE](https://www.trae.ai/)** (zzgl. [TRAE Solo](https://www.trae.ai/solo))
		- More: **[Void](https://voideditor.com/)**, [Tabby](https://www.tabbyml.com/), [Qodo Command](https://www.qodo.ai/products/qodo-command/)/[Qodo Gen](https://www.qodo.ai/products/qodo-gen/)
		- ReactJS/UI-centric: [Onlook](https://onlook.com/)
		- UI-Design: [SuperDesign.Dev](https://www.superdesign.dev/)
	- VS Code Extensions:
		- **[TabNine](https://www.tabnine.com/install/vs-code/)** (kostenlos ist nur die Short-Code-Completion)
		- GitHub [Copilot VS Code Extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)
		- OpenAI Codex als VS Code Extension: **[Code GPT](https://marketplace.visualstudio.com/items?itemName=DanielSanMedium.dscodegpt)**)
		- [Kudo](https://www.kodu.ai/)
	- Cloud:
		- Universal: [replit](https://replit.com/), Google [jules](https://jules.google/), Google [AI Studio](https://aistudio.google.com)
		- Web&Mobile in General: [bolt](https://bolt.new/), [biela.dev](https://biela.dev/), [shelbula.dev](https://shelbula.dev/), [JDoodle.ai](https://www.jdoodle.ai/)
		- ReactJS: [loveable](https://lovable.dev/), [Tempo](https://www.tempo.new)
		- Next.js: [v0](https://v0.dev/chat) (UI-centric)
		- GitHub **[Copilot](https://github.com/copilot/)**
		- Weiterführende Liste: [AI Tools Club](https://aitoolsclub.com/top-50-ai-vibe-coding-tools-for-everyone-in-2025/)
	- Nennenswerte weitere Ansätze:
		- [MetaGPT](https://github.com/FoundationAgents/MetaGPT): Multi-Agent Framework that assigns different roles to GPTs to form a collaborative entity for complex tasks ([Docs](https://docs.deepwisdom.ai/main/en/guide/get_started/introduction.html))
			- MetaGPT X (= Spin-off product by MetaGPT inventors): [MGX](https://mgx.dev/)
- MCP
	- MCP Repository: [smithery.ai](https://smithery.ai/)
- Für SQL (KI-gestützte SQL Code-Completion)
	- Open-Source **[NSQL](https://huggingface.co/NumbersStation)** mit [Begleitartikel](https://www.numbersstation.ai/post/introducing-nsql-open-source-sql-copilot-foundation-models)
	- Kostenpflichtig (€): **[Cogram](https://www.cogram.com/)**
- Vibe Testing
	- [RobotFramework](https://robotframework.org/) als Testökosystem, da dessen Testbeschreibungen sehr natürlichsprachlich sind
	- [Harness AI Test Automation](https://www.harness.io/products/ai-test-automation)
	- [testRigor](https://testrigor.com/) (free for public open source)
	- Teilaspekt von [Qodo Gen](https://www.qodo.ai/products/qodo-gen/)
	- Java-centric: [diffblue](https://www.diffblue.com/)
	- Webartikel: Vibe Testing [with Playwright](https://timdeschryver.dev/blog/vibe-testing-with-playwright)
- Vibe Hacking / Vibe Pentesting
	- Local/CLI: [vulnhuntr](https://github.com/protectai/vulnhuntr)
	- Cloud/GUI: [Vibe Coding Penetration Tester](https://github.com/firetix/vibe-coding-penetration-tester) (cf. [vibehack.io](http://vibehack.io/)), [ZeroThreat](https://zerothreat.ai/)
- Vibe Coding via Prompting
	- Tutorials: [loveable](https://docs.lovable.dev/tips-tricks/prompting-one), [VibeCoding](https://github.com/cpjet64/vibecoding/tree/main), [bolters.io Knowledge Base](https://bolters.io/)
	- Prompting Recipies: Prompting Library by [loveable](https://docs.lovable.dev/prompting/prompting-library), [cursor.directory](https://cursor.directory/rules), Examples by [VibeCodex](https://vibecodex.io/#prompts), OpenAI Academy [Prompt Packs](https://academy.openai.com/public/tags/prompt-packs-6849a0f98c613939acef841c)
	- Prompt Generators: [TinyToolStack](https://tinytoolstack.com/app/vibecodingpromptgenerator?ref=producthunt), PromptHub [Prompt Iterator](https://www.prompthub.us/prompt-enhancers/prompt-iterator), [Bolt Prompter](https://chatgpt.com/g/g-tozliiBeO-bolt-prompter)
- Supporting Tools
	- Pack your codebase into AI-friendly formats: [Repomix](https://repomix.com)
- Weiterführende Referenzen: [Awesome Vibe Coding](https://github.com/filipecalegario/awesome-vibe-coding), [Awesome Vibe Coding Tools](https://github.com/furudo-erika/awesome-vibe-coding-tools?tab=readme-ov-file) 



## SW-Bibliotheken & -Frameworks

- für **[Python](https://github.com/vinta/awesome-python)**
- für **[Java](https://github.com/akullpp/awesome-java)**
- für C#: **[.NET Core](https://github.com/thangchung/awesome-dotnet-core)** bzw. **[.NET Framework](https://github.com/quozd/awesome-dotnet)**
- für **[JavaScript](https://github.com/sorrycc/awesome-javascript)**
- für **[Node.js](https://github.com/sindresorhus/awesome-nodejs)**
- für **[C++](https://github.com/fffaraz/awesome-cpp)**
- für **[PHP](https://github.com/ziadoz/awesome-php)**

## Testing

- Code Coverage Selbstcheck? Code Coverage Analyzer ⚠️, wie bspw. **[EclEmma](https://www.eclemma.org/)** (Java), **[Istanbul](https://istanbul.js.org/)** (JS), **[coverlet](https://github.com/coverlet-coverage/coverlet)** (C#), etc.pp
	- Weiterführende Referenzen: Blogartikel [The Best Code Coverage Tools By Programming Language](https://about.codecov.io/blog/the-best-code-coverage-tools-by-programming-language/)
- [**ArchUnit** Java](https://www.archunit.org/) | **[ArchUnitNET](https://github.com/TNG/ArchUnitNET/)**: Unit test your architecture
- **[Testcontainers](https://www.testcontainers.org/)**: Java-Bibliothek zur leichtgewichtigen Testintegration von Datenbanksystemen, NoSQL-Systemen, Webservern, Log-Diensten u.a.
- SQL-Testing / Testing Frameworks, wenn man selbst eine DBMS-Engine entwickelt: **[SQLsmith](https://github.com/anse1/sqlsmith)** für Query Fuzzing | **[SQLancer](https://github.com/sqlancer/sqlancer)** für SQL Logik Verifikation | **[SQL Logic Tests](https://www.sqlite.org/sqllogictest/doc/trunk/about.wiki)** from SQLite
- **[Jest](https://jestjs.io/)**: JavaScript Unit-Testing ([Cheat Sheet](https://devhints.io/jest))
- Test web UI components in a user-centric way: **[Testing Library](https://testing-library.com/docs/)**
- **[Ponicode Unit Tests](https://www.npmjs.com/package/ponicode)**: Unit-Test-Generator für JavaScript und Python
- **[WireMock](https://wiremock.org/)**: Mock Web-APIs, i.a., gRPC
- **[Mock Service Worker (MSW)](https://mswjs.io/)**: library for Web-API mocking
- WebApp End-to-End (E2E) Testing
	- **[Cypress](https://www.cypress.io/)** \[**choco install cypress**\]: open source testing for anything that runs in a browser, Fokus: JavaScript
	- **[PlayWright](https://playwright.dev/)**: testing for modern web apps (Open Source, von Microsoft), eher Multi-Language i.S.v. JavaScript, Java, Python und C#
	- **[Protractor](https://www.protractortest.org)** speziell für AngularJS und Angular
	- (Weitere Alternativen: Selenium, …)
- AI-powerd E2E Test Automation: **[testRigor](https://testrigor.com/)**, kostenlos für public open source | **[testIM](https://www.testim.io/)** mit kostenlosen Kontingenten
- Load-Testing
	- (Web/Self-Hosted:) [**Gatling** Open Source](https://gatling.io/open-source/)
	- (Desktop:) **[JMeter](https://jmeter.apache.org/)** \[choco install jmeter\]
	- (CLI:) **[k6](https://k6.io/open-source/)** \[choco install k6\]
- **[Cucumber](https://cucumber.io/docs/installation/)**: BDD-Testing
- **[Kiwi TCMS](https://github.com/kiwitcms/Kiwi)**: Open Source Test Case Management System
- A/B-Testing-on-Steroids: **[Split](https://www.split.io/)** für Web-Anwendungen
- Fuzz Testing: bspw. [Jazzer](https://github.com/CodeIntelligenceTesting/jazzer) (Java) oder [JQF+Zest](https://github.com/rohanpadhye/JQF) (Java)
- Weiterführende Quellen: [Awesome Test Automation](https://github.com/atinfo/awesome-test-automation) | [Awesome Testing](https://github.com/TheJambo/awesome-testing) | [Awesome Android Testing](https://github.com/hotchemi/awesome-android-testing)

## Fehleranalyse

- Debugging
	- **[dnSpy](https://github.com/dnSpy/dnSpy)** (auch [Portable per ZIP](https://github.com/dnSpy/dnSpy/releases)): **Portable** .NET debugger (und .NET assembly editor, s. unten)
- Netzwerk
	- **[NETworkManager](https://borntoberoot.net/NETworkManager/)** ⭐ \[**choco install networkmanager --ignore-dependencies**\]: Windows Werkzeug für die Netzwerk-Analyse (ping, traceroute, IP scanner, Portscanner, uvm.)
	- ggf. **[Wireshark](https://www.wireshark.org/)** \[**choco install wireshark**\] und **[nmap](https://nmap.org/)** \[**choco install nmap**\]
	- Bandbreitenmessung (throughput): **[iperf3](https://iperf.fr/)** ⭐ \[**choco install iperf3**\] (must run iperf3 server on backend target host)
		- (Im professionallen Bereich weniger nützlich, da nur Lokaler-Rechner-zu-eigenem-ISP: LibreSpeed [librespeed-cli](https://github.com/librespeed/speedtest-cli) \[**choco install librespeed-cli**\], Ookla [speedtest-cli](https://www.speedtest.net/apps/cli) \[**choco install speedtest**\])
- Logging
	- **[Baretail](http://www.baremetalsoft.com/baretail/)** \[**choco install baretail**\]: Windows Werkzeug für Real-time Log-File Monitoring (USP: auch **Portable**)
	- **[Tail Blazer](https://github.com/RolandPheasant/TailBlazer)** \[**choco install tailblazer**\]: Windows Werkzeug für Real-time Log-File Monitoring (USP: auch **RegExp**)
- Umgebungsvariablen
	- **[RapidEE](https://www.rapidee.com)** \[**choco install rapidee**\]: Windows Environment Variables Editor
- Decompiler
	- **[dnSpy](https://github.com/dnSpy/dnSpy)** \[**choco install dnspy --ignore-dependencies**\]: .NET assembly editor (und .NET debugger, s. oben)
	- **[Java-Decompiler](http://java-decompiler.GitHub.io/)** \[**choco install javadecompiler-gui**\]: Java decompiler

## Wireframing & Prototyping & UX

- **[Uizard](https://uizard.io/)**: Cloud-basiertes Wireframing & Prototyping Werkzeug (wie Figma et al.), aber mit KI-Komponente: Es kann Handzeichnungen in einen Prototypen umwandeln (sog. [Design Assistant](https://uizard.io/design-assistant/))
	- **[Figma](https://www.figma.com/)** als Cloud-Anwendung
		- Figma ist kostenlos für [Studierende](https://www.figma.com/education/)
	- Alternativen: [mydraft](https://mydraft.cc/), [Moqups](https://moqups.com/), [Framer](https://www.framer.com/), [NinjaMock](https://ninjamock.com/), uvm.
	- (Vorsicht vor **[JustInMind](https://www.justinmind.com)**: Ein sehr gutes Wireframing/Prototyping-Tool, zunächst kostenlos, aber nach 2 Monaten, was nicht in der Pricing-Übersicht steht, verliert man eine Vielzahl von Möglichkeiten und danach ist JustInMind m.E. unbrauchbar)
	- **[Adobe XD](https://www.adobe.com/de/products/xd.html)** als Desktop-Anwendung, auch für Web & Mobile, aber seit einiger Zeit von Adobe aufgebeben
- **[Pencil Project](https://pencil.evolus.vn/)**: Open Source GUI Prototyping
- Personas:
	- Deutsch: **[Make My Persona](https://www.hubspot.de/make-my-persona)**
	- Englisch: **[SEMRush](https://de.semrush.com/persona/)**, [UserForge](https://userforge.com/) (free: 2 Personas) [UXPressia Persona Creator](https://uxpressia.com/personas-online-tool) (free: 1 Persona), [PersonaGenerator](https://personagenerator.com/) oder [Xtensio](https://xtensio.com/user-persona-template/)
	- KI-gestützter Generator (auf Basis von Google Analytics Daten): **[delve.ai](https://www.delve.ai/live-persona)**
	- Portrait-Bilder: **[This Person Does Not Exist](https://thispersondoesnotexist.com/)** (oder [Pexels](https://www.pexels.com/) sowie [Unsplash](https://unsplash.com/de))

## Modellierung & Architektur

- **[PlantUML](https://plantuml.com/)** ⭐⭐⭐
	- Eigenschaften: Diagrams-as-Code / git-fähig / Kommandozeilen-Anwendung / auf Basis einer textuellen Notation
	- Desktop: **choco install plantuml** | Cloud: **[planttext.com](https://www.planttext.com)**
	- [Wofür](https://plantuml.com/sitemap-language-specification)?
		- UML ⭐: [Komponenten](https://plantuml.com/component-diagram) ⭐, [Klassen](https://plantuml.com/class-diagram) ⭐, [Sequenz](https://plantuml.com/sequence-diagram) ⭐, [Use-Case](https://plantuml.com/use-case-diagram) ⭐, [Deployment](https://plantuml.com/deployment-diagram), [State-Charts](https://plantuml.com/state-diagram)
		- [Entity/Relationship-Diagramme](https://plantuml.com/er-diagram) ⭐ in Chen-Notation sowie auch EE/R (inkl. Vererbung)
		- [JSON](https://plantuml.com/json) ⭐ und [YAML](https://plantuml.com/yaml)
		- [Wireframes](https://plantuml.com/salt) ⭐ in der UI/UX-Konzeption
		- [Organigramme](https://plantuml.com/wbs-diagram) ⭐ und gleichsam [Projektstrukturplan (PSP)](https://plantuml.com/wbs-diagram)
		- [Syntaxdiagram via EBNF](https://plantuml.com/ebnf) also erweiterter Backus-Naur-Form (EBNF)
		- [Netzwerkdiagramme](https://plantuml.com/nwdiag)
		- [MindMap](https://plantuml.com/mindmap-diagram)
	- Nennenswert #1: Wie handgezeichnet mit „[skinparam handwritten true](https://plantuml.com/handwritten)“
	- Nennenswert #2: Sequenzdiagramme auch in [ASCII-Art](https://plantuml.com/ascii-art)
	- Nennenswert #3: LaTeX-Einbindung: CTAN [plantuml](https://ctan.org/pkg/plantuml) package
	- Nennenswert #4: [Konvertierung von Quellcode nach PlantUML: **gituml.com**](https://gituml.com/listz)
	- Auswahl an Extensions: [C4 model](https://github.com/plantuml-stdlib/C4-PlantUML) ⭐, [AWS](https://github.com/awslabs/aws-icons-for-plantuml) ⭐, [Azure](https://github.com/plantuml-stdlib/Azure-PlantUML) ⭐, ...
	- Cloud-Beispiele: [Hitchhiker's Guide to PlantUML](https://crashedmind.GitHub.io/PlantUMLHitchhikersGuide/aws/aws.html)
	- Web-zentrische Alternativen: **[Mermaid](https://mermaid-js.GitHub.io/mermaid/#/entityRelationshipDiagram)** JavaScript-Bibliothek
- **[Mermaid](https://mermaid.js.org)** ⭐: ähnlich geil wie PlantUML
	- Mittlerweile nicht nur als JS-Bibliothek sondern auch als lokales [CLI-Werkzeug](https://github.com/mermaid-js/mermaid-cli) \[npm install -g @mermaid-js/mermaid-cli\], das bspw. SVGs erzeugt
	- Überdeckung mit PlantUML: [UML](https://mermaid.js.org/syntax/zenuml.html) und [MindMaps](https://mermaid.js.org/syntax/mindmap.html)
	- Unterstützt in Ergänzung zu PlantUML noch einige [andere Diagrammarten](https://mermaid.js.org/intro/) ⭐, bspw. [QuadrantCharts](https://mermaid.js.org/syntax/quadrantChart.html), [git-Graphen](https://mermaid.js.org/syntax/gitgraph.html), [Paket-Diagramme](https://mermaid.js.org/syntax/packet.html) und [Sankey-Diagramme](https://mermaid.js.org/syntax/sankey.html) sowie [Kanban-Diagramme](https://mermaid.js.org/syntax/kanban.html)
- (Mit [draw.io/diagrams.net](https://drawio-app.com/) bzw. Microsoft Visio kann man natürlich ein [Klassendiagramm](https://drawio-app.com/uml-class-diagrams-in-draw-io/) zeichnen)
- **[Cloudcraft](https://www.cloudcraft.co)**: Visualisierung von Cloud-Architekturen. Als Cloud-WebApp. ([Beispiele](https://www.google.com/search?q=cloud+architecture+cloudcraft&tbm=isch))
	- Unterstützt auch [Export nach draw.io/diagrams.net](https://www.diagrams.net/blog/drawio-aws-cloudcraft)
- REST-Schnittstellen dokumentieren?
	- OpenAPI: **[Swagger](https://editor.swagger.io/)** ([Editor](https://editor.swagger.io/) und [Beispiel](https://petstore.swagger.io/))
		- Reverse Engineering von einer bestehenden App: [mitmproxy2swagger](https://github.com/alufers/mitmproxy2swagger) ([Tutorial-Webartikel](https://medium.com/@amaraltohami30/reverse-engineer-an-api-using-mitmweb-and-postman-and-create-a-swagger-file-crapi-99f01b58511c))
		- YAML-to-LaTeX? (1) [YAML-to-MD](https://github.com/OpenAPITools/openapi-generator-cli) \[npm install @openapitools/openapi-generator-cli\] (2) Cloud-based [Aspose md-to-tex](https://products.aspose.app/pdf/conversion/md-to-tex)
- Event-Driven Architecture / Asynchronous APIs dokumentieren? (WebSockets, Kafka, ...)
	- **[AsyncAPI](https://www.asyncapi.com/)** ([Editor](https://studio.asyncapi.com) und [Übersicht](https://www.asyncapi.com/docs/tutorials/getting-started/coming-from-openapi))
- **[Visual Paradigm](https://www.visual-paradigm.com/)** [Community Edition](https://www.visual-paradigm.com/download/community.jsp): UML, SysML, AWS/Azure/GCP Architekturdiagram, uvm.
	- (Unter Windos bspw. mittels chocolatey: **choco install visualparadigm-ce**)
	- (€:) [Nur ab Standard Edition](https://www.visual-paradigm.com/editions/): Kostenpflichtige [**Code Generation/Reversal** für Java, C++, C#, SQL, **Python**, uvm.](https://www.visual-paradigm.com/features/code-engineering-tools/) (aber kein JavaScript)
	- Cloud-Alternative: **[Visual Paradigm Online](https://online.visual-paradigm.com/de/diagrams/partner/academic/)**
- **[Modelio](https://www.modelio.org/)**: Open-Source und Eclipse-basiert; UML, SysML, BPMN und TOGAF-bezogene Diagrammarten
	- (Unter Windos bspw. mittels chocolatey: **choco install modelio**)
	- Kostenlose [**Code Generation/Reversal**: Java, C++, C# und SQL](https://www.modeliosoft.com/en/features/model-driven-code-generation.html) (sonst nix, bspw. kein Python; auch kein JavaScript)
- **[Kroki](https://kroki.io)** Server: u.a. UML / Diagrams-as-Code / git-fähig / URL-Anwendung / auf Basis textueller Notationen
	- Unified API with support for PlantUML, BlockDiag, BPMN, Bytefield, C4, Ditaa, Erd, Excalidraw, GraphViz, Mermaid, Nomnoml, Pikchr, Structurizr, SvgBob, UMLet, Vega, Vega-Lite, WaveDrom
	- Beispiele: [Liste verschiedener Diagramme](https://kroki.io/examples.html)
- JavaScript UML Generator? (derzeit: nur UML Klassendiagramme)
	- **[arkit](https://www.npmjs.com/package/arkit)**: Kommandozeilen-Werkzeug für JavaScript und TypeScript, das primär PlantUML generiert (und daraus abgeleitet SVG oder PNG)
	- **[TsUML](https://github.com/remojansen/TsUML)**: Kommandozeilen-Werkzeug für TypeScript (basierend auf yuml.me)
	- JetBrains [WebStorm](https://www.jetbrains.com/webstorm/) (InteliJ-basiert) mit dem Plugin **[UML JavaScript and TypeScript](https://plugins.jetbrains.com/plugin/17380-uml-javascript-and-typescript)**
	- [Eclipse](https://www.eclipse.org) mit der Extension **[JS/UML](https://jsuml.sourceforge.net)**
- **[DSM Suite](https://dsmsuite.GitHub.io/dsm_overview)**: managing software dependencies using a design structure matrix
- **[Camunda Modeler](https://camunda.com/download/modeler/)**: Für Workflow-Modellierung mittels BPMN, Open-Source
	- (Unter Windos bspw. mittels chocolatey: **choco install camunda-modeler**)
	- Cloud-Variante: **[bpmn.io](https://bpmn.io/)**
- **[Archi](https://www.archimatetool.com/download/)**: [TOGAF](https://www.opengroup.org/togaf)-bezogene Diagrammarten
	- (Archi nicht über chocolatey beziehen; die dortige Version ist schon lange veraltet)
- **[Madge](https://github.com/pahen/madge)**: Visualisierung eines JavaScript dependency-trees mittels graphviz
- **[Structurizr](https://structurizr.com/)**: [C4-Model](https://en.wikipedia.org/wiki/C4_model)-bezogene Diagrammarten, bspw. auch für Cloud Architekturen
- **[LucidChart](https://www.lucidchart.com/)**: Sehr mächtiges Cloud-basiertes Zeichen- und Modellierungswerkzeug
	- Leider sind nur 3 Dokumente kostenlos
- **Entity/Relationship-Modellierung** (ERM) = konzeptionelle Datenmodellierungsebene
	- aka: Entity/Relationship-Diagramme (ERD) sowie erweiterte Entity/Relationship-Diagramme (EER) nach Elmasri & Navathe
	- Top ⭐: [PlantUML](https://plantuml.com/er-diagram)
	- Cloud:
		- **[PlantUML](https://editor.plantuml.com/uml/SoWkIImgISv8pUFYIiqhoIofL0X8BIhEprEevgg5YVZa9oUMP4B5Yb9pm9pYZCm21QVCefACWfp4v5Im71TKhwwVBf8K5v8gNKDTk75SN0wfUIbWkm40)**
		- **[ERDplus](https://erdplus.com/)** ⭐: Bestes Cloud-basiertes E/R-Werkzeug
		- Schöne [E/R-Diagramme per **draw.io**](https://drawio-app.com/entity-relationship-diagrams-with-draw-io/) \[**choco install drawio**\]
		- **[Mermaid](https://mermaid-js.GitHub.io/mermaid/#/entityRelationshipDiagram)**
		- Handzeichnungsstil: [excalidraw](https://excalidraw.com/)
		- Weitere Alternativen mit starker Limitierung der Free Plans: [creately](https://creately.com/lp/er-diagram-tool-online/), etc.
	- Desktop:
		- **[PlantUML](https://plantuml.com/er-diagram)** ⭐ mit E/R in Chen-Notation sowie auch EE/R also inkl. Vererbung
		- Microsoft Visio mittels [meiner eigenen E/R **Visio-Stencils**](http://www.cyberlytics.eu/theses/templates/ERD-Chen76_EERD-ElmasriNavathe94.vss) für die Chen-Notation sowie für erweiterte E/R-Diagramme nach Elmasri
		- [Oracle **SQL Developer**](https://www.oracle.com/database/sqldeveloper/)
			- mittels eines [Oracle Accounts](https://profile.oracle.com/myprofile/account/create-account.jspx) \[**choco install oracle-sql-developer --ignore-dependencies --params "'/Username:{oraUser} /Password:{oraPwd}'"**\] dabei ist der {oraUser} i.d.R. eine E-Mail-Adresse und die geschweiften Klammern sind nicht Teil der Syntax sondern nur Platzhaltersymbolik
	- **Warnhinweis**: Viele amerikanischen Tools (u.a. MySQL-Workbench, [dbdiagram.io](https://dbdiagram.io/), etc. pp.) behaupten fälschlicherweise, Sie würden E/R-Diagramme darstellen, aber oft ist die Notation nur eine Visualisierung von Relationen und diese Tools erlauben keine konzeptionelle Modellierung nach dem E/R-Modell
- DB **Schema Diagram** = logische Datenmodellierungsebene: Relationen
	- aka: Database Schema Diagram, Relational Diagram, Database Relationship Diagram, Schema Model, Schema Design (Mr. Obvious: es hat sich leider nie eine einheitliche Bezeichnung für diesen Typ von Diagramm gebildet) (und deswegen werden diese Diagramme häufig mit E/R fälschlich in einen Topf geworfen)
	- Cloud: [ChartDB](https://chartdb.io/)
		- Stark limitiert in der Free Edition (i.d.R. 10 bis 15 Tabellen, kann aber für eine Bachelor-/Masterarbeit reichen): [azimutt](https://azimutt.app/pricing), [drawSQL](https://drawsql.app/#pricing), [QuickDBD](https://www.quickdatabasediagrams.com/#pricing), [DB Designer](https://www.dbdesigner.net/plans/)
		- Unter dem fehlgeleiteten Begriff E/R-Diagram: [dbdiagram.io](https://dbdiagram.io/), [cacoo](https://nulab.com/cacoo/examples/database-diagrams-er-diagram-tool/)
	- Desktop: [Jetbrains **DataGrip**](https://www.jetbrains.com/datagrip/features/) (kostenlos für Studierende)
		- Unter dem fehlgeleiteten Begriff E/R-Diagram: [MySQL-Workbench](https://www.mysql.com/products/workbench/), u.a.
- NoSQL Document Diagrams
	- aka: Nested Columns Diagram (auch hier gibt es derzeit keine Normung, weder zur Bezeichnung der Diagramme, noch zur Visualisierungsform)
	- **[DbGate](https://dbgate.org)** \[**choco install dbgate.portable**\]: Open-Source Cross-Plattfrom SQL+NoSQL Editor (inkl. starkem JSON-Viewer)
	- **[azimutt](https://azimutt.app/blog/exploring-document-databases-with-azimutt)** erlaubt die Visualisierung von Document Stores \[npx azimutt export mongodb "mongodb://user:password@localhost"\]
- JSON-Modellierung
	- JSON-Dokument-Visualisierung: [PlantUML](https://plantuml.com/json) ⭐
	- JSON ist zunächst schemalos und die wenigen Sprachen zur Spezifikation von Web-APIs (z. B. [Swagger](https://swagger.io/), [RAML](http://raml.org/)) erlauben die Spezifikation von API-Diensten und ihren Parametern, aber keine konzeptionelle Visualisierung das vollständige API-Schema
	- ABER: Das **konzeptionelle Schema** von **JSON**-Dokumenten kann man genauso **mit Entity/Relationship-Diagrammen** oder **mit UML** darstellen!
		- (Auch selten genutzte Spezifikationsmöglichkeiten wie [JSON Schema](http://json-schema.org) sind m.E. weder durch Modellierungswerkzeuge gestützt noch gibt es Round-Trip support zur Extraktion von Schemainformation aus Dokumentinstanzen rund um JSON Schema)
	- TIPP #1 (wie oben bereits): [PlantUML](https://plantuml.com/json) ⭐
	- TIPP #2: Visualisieren Sie das Schema, das sich hinter Ihren JSON-Dokumenten verbirgt, in UML mit **[JSON discoverer](http://som-research.uoc.edu/tools/jsonDiscoverer/#/)**
	- TIPP #3: **[DbGate](https://dbgate.org)** ist ein SQL+NoSQL Editor, aber integriert ebenfalls einen starken JSON-Viewer
- **ASCII**-basierte Diagramme
	- UML-Klassendiagramm: **[TextUML](http://abstratt.GitHub.io/textuml/index.html)**
	- UML-Squenzdiagramm: **[PlantUML](https://plantuml.com/ascii-art)**
	- Diverse ASCII-Visualisierungen: **[Diagon](http://arthursonzogni.com/Diagon/)** (Sequenzdiagramme, Bäume, Tabellen, Graphen, Flowcharts, …)
	- ASCII-Kunst-Generator: **[rexpaint](https://www.gridsagegames.com/rexpaint/)**
- KI-gestützte Modellierung:
	- **[ChatUML](https://chatuml.com)**
	- Webartikel [**ChatGPT** — How to Generate UML Diagram](https://blog.devgenius.io/chatgpt-how-to-generate-uml-diagram-cb745ecba83e) (indem man sich PlantUML-Text generieren lässt)
- **Software-Archäologie** und -Visualisierung:
	- Open Source: **[Sourcetrail](https://github.com/CoatiSoftware/Sourcetrail/)** \[**choco install sourcetrail**\]
	- Kostenpflichtig aber **nennenswert: [Lattix](https://www.lattix.com/)**, | **[Sonargraph](https://www.hello2morrow.com/products/sonargraph)** (früher: SotoGraph/SotoArc) | **[Structure101](https://structure101.com/)** | **[JArchitect](https://www.jarchitect.com/)** | **[NDepend](https://www.ndepend.com/)**
- Weiterführende Quelle: [Awesome Software Architecture](https://awesome-architecture.com/) | [Awesome Diagramming](https://github.com/shubhamgrg04/awesome-diagramming) | [AWS Architecture Blueprints](https://aws.amazon.com/architecture/) | [Survey of Architecture Frameworks](http://www.iso-architecture.org/ieee-1471/afs/frameworks-table.html)

## DevOps

\[Hier: traditionell, d.h. grundlegende DevOps-Bausteine! Cloud-spezifische Sicht: vgl. BDCC/AI-Schwesterseite zu [Cloud-native DevOps](https://github.com/cyberlytics/awesome-bdccai-tools#devops) (!)\]

- Vergleiche andere Abschnitte
	- **[git](#git)** wg. GitOps
	- [kostenlosen Alternativen](#kostenlose-alternativen) für **Atlassian**-Substitutionen
- SysOps / SysAdmin
	- Weiterführende Quellen: [Awesome Sysadmin #1](https://github.com/kahun/awesome-sysadmin) | [Awesome Sysadmin #2](https://github.com/awesome-foss/awesome-sysadmin) | [Libhunt: SysAdmin](https://sysadmin.libhunt.com/)
- Dependency Management:
	- Software Bill of Materials (SBOM): [Awesome SBOM](https://github.com/awesomeSBOM/awesome-sbom)
- Build-Automatisierung
	- Build-Werkzeuge:
		- Monorepo-zentrisch: [Monorepo-Build-Werkzeuge](https://monorepo.tools) | [Awesome Monorepo](https://github.com/korfuri/awesome-monorepo)
		- Polyrepo-/Multirepo-zentrisch: Liste [Managing multi-git repositories efficiently](https://gist.github.com/mahmoudimus/fd71c95dc7d7a99056186466623d883f) | npm [polyrepo](https://github.com/polyrepo/polyrepo) | npm [meta](https://github.com/mateodelnorte/meta) | [**GitKraken** mit Multi-Repo-Unterstützung](https://www.gitkraken.com/blog/git-multi-repo-vs-git-mono-repo)
	- Git Hooks
		- **[Husky](https://typicode.GitHub.io/husky/#/)**: Modern native git hooks made easy
		- Vorlagen: **[Awesome Git Hooks](https://github.com/CompSciLauren/awesome-git-hooks)**
		- **[GitHub Actions](https://docs.docker.com/build/ci/github-actions/)**
	- Java Builds
		- Als Bestandteil meines Dissertationsprojekt habe ich eine Java-Build-Referenz auf Basis von Maven geschaffen: [cpnatwork/alphaflow_dev](https://github.com/cpnatwork/alphaflow_dev/tree/master/sys-src) (mit einem \*-buildhub-Modul für die Build-Komposition und mit \*configbase-Modulen für Abhängigkeitskonsolidierung mittels Maven-POM-Vererbung)
	- C# Builds
		- .NET Framework (C#): [MSBuild Binary and **Structured Log Viewer**](https://msbuildlog.com/) \[**choco install msbuild-structured-log-viewer** -y --ignore-dependencies\]: Viewer for .binlog files from „MSBuild.exe /bl“
		- **[NuGet](https://learn.microsoft.com/nuget/)** \[**choco install nuget.commandline**\]: Blogeintrag **[5 steps to better NuGet package](https://alex-klaus.com/better-nuget/)** von Alex Klaus
			- [NuGet Package Explorer](https://github.com/NuGetPackageExplorer/NuGetPackageExplorer) \[**choco install nugetpackageexplorer**\]
			- [NuGetDefense](https://digitalcoyote.GitHub.io/NuGetDefense/) \[**choco install nugetdefense**\]: checks for known vulnerabilities; inspired by OWASP SafeNuGet
		- **[il-repack](https://github.com/gluck/il-repack)** \[**choco install il-repack**\]: improved version of ILMerge / Mono.Merge, for replacing them
		- [**semver**.net](https://github.com/adamreeve/semver.net): library that implements the [Semantic Versioning specification](http://semver.org/) and the version range specifications used by npm
		- **[Paket](https://fsprojects.GitHub.io/Paket/)** \[**choco install paket**\]: dependency manager for .NET with support for NuGet packages and Git repositories
	- Tools:
		- **[FastPack](https://github.com/QuanosSolutions/FastPack)**: deduplication (de)compressor that is particularly useful for compressing and decompressing build artifacts
- API Management:
	- [**gravitee**.io](https://www.gravitee.io/pricing): Open Source API management platform
- **Continuous Integration**
	- [Awesome CI](https://github.com/ligurio/awesome-ci)
- **Continuous Delivery**
	- **[Awesome CI and CD](https://github.com/cicdops/awesome-ciandcd)**
	- (Thema auch in [Awesome CI](https://github.com/ligurio/awesome-ci) tlw. inkludiert)
- Lizenzen:
	- Lizenz-Checker für den Software Bill of Materials: **[FOSSA](https://fossa.com)**
- Software-Artifact Repository \[Web/Self-Hosted\]
	- [Sonatype **Nexus**](https://de.sonatype.com/products/repository-oss-download) (OSS-Version)
	- Inedo **[ProGet](https://inedo.com/proget/download)** (Free Version)
- [Graphviz](https://www.graphviz.org/download/) **[dot](https://graphviz.org/doc/info/lang.html)** \[choco install graphviz\]: graph description language
- **ITSM**:
	- «Open Source» **[Zammad](https://zammad.org/)**
	- «Empfehlung(€€€)» **[ServiceNow](https://www.servicenow.com/)** (Leader im Gartner [Magic Quadrant for IT Service Management Platforms](https://static.ivanti.com/sites/marketing/media/images/misc/ivanti-gartner-itsm-mq-2022.png))
- **Cloud-native DevOps**: vgl. BDCC/AI-Schwesterseite [DevOps](https://github.com/cyberlytics/awesome-bdccai-tools#devops)
- **MLOps**: vgl. BDCC/AI-Schwesterseite zu [ML / AI](https://github.com/cyberlytics/awesome-bdccai-tools#ml--ai)
- **DevSecOps**: vgl. BDCC/AI-Schwesterseite zu [Security](https://github.com/cyberlytics/awesome-bdccai-tools#security)
- Weiterführende Quellen (traditionell/grundlegend):
	- [Awesome DevOps #1](https://github.com/wmariuss/awesome-devops), [Awesome DevOps #2](https://github.com/awesome-soft/awesome-devops), [The Book of Secret Knowledge](https://github.com/trimstray/the-book-of-secret-knowledge)
	- - (Cloud-native Quellen auf der [BDCC/AI-Schwesterseite](https://github.com/cyberlytics/awesome-bdccai-tools#devops))

## Software-Internationalisierung (I18n) & -Lokalisierung (L10n)

- Wichtige Aspekte: Pluralization & Gender
- Technischer Einstieg **am Beispiel Java**: Baeldung [Guide to Internationalization in **Spring Boot**](https://www.baeldung.com/spring-boot-internationalization) (2022)
- Technologie
	- Webartikel [Common Localization File Formats](https://www.transifex.com/blog/2016/common-localization-file-formats/) (2016): PO, XLIFF, RESX, Android-XML, Java Properties, JSON, CSV
	- [GNU gettext / PO file](https://www.gnu.org/software/gettext/manual/gettext.html):
		- C/C++: [GNU gettext and libintl](https://erri120.GitHub.io/posts/2022-05-05/)
		- Java: [gettext-commons](https://github.com/jgettext/gettext-commons)
		- JS: [gettext.js](https://github.com/guillaumepotier/gettext.js/)
		- Py: [gettext](https://docs.python.org/3/library/gettext.html)
		- C#: (.NET hat eine umfangreiche i18n Lokalisierung eingebaut)
	- [ICU](https://icu.unicode.org/):
		- C/C++: [ICU4C](https://unicode-org.GitHub.io/icu/userguide/icu4c/)
		- Java: [ICU4J](https://unicode-org.GitHub.io/icu/userguide/icu4j/), vgl. Baeldung [Java Localization – Formatting Messages](https://www.baeldung.com/java-localization-messages-formatting) (2023)
		- JS: [messageformat](https://github.com/messageformat/messageformat)
		- Py: [PyICU](https://pypi.org/project/PyICU/) (mittels ICU C++)
	- Nennenswerte Programmiersprachen-individuelle Techniken:
		- Java: [ResourceBundle](https://docs.oracle.com/javase/tutorial/i18n/resbundle/concept.html)-Dateien
		- C#: [resx](https://learn.microsoft.com/en-us/dotnet/core/extensions/work-with-resx-files-programmatically)-Dateien (.NET hat eine umfangreiche [Globalisierung/Lokalisierung](https://learn.microsoft.com/en-us/dotnet/core/extensions/globalization-and-localization?redirectedfrom=MSDN) eingebaut)
		- Py: [YAML](https://guides.rubyonrails.org/i18n.html)- oder Ruby-Dateien per [Rails I18n gem](https://guides.rubyonrails.org/i18n.html), in generic Py per [python-i18n](https://pypi.org/project/python-i18n/)
- Essential Toolkit for Localization Engineers: **[Translate Toolkit](https://github.com/translate/translate)** mit diversen Datei-Konvertern
- **[simplelocalize-cli](https://simplelocalize.io/docs/cli/i18n-keys-extraction/)**: Extract translation keys and messages from various different libraries
- **[GitLocalize](https://gitlocalize.com/)**: localization tool for GitHub repository (e.g. MD files)
- **[OmegaT](https://omegat.org)** \[**choco install omegat**\]: free translation memory tool
- **[CheckMate](https://okapiframework.org/wiki/index.php?title=CheckMate)**: Cross-platform application that allows you to perform various quality checks on bilingual translated documents
- Weiterführende Quelle: [Awesome Translations](https://github.com/mbiesiad/awesome-translations), [Awesome I18N](https://github.com/jpomykala/awesome-i18n)

## Quantencomputing

- **[qiskit](https://qiskit.org)**: open-source toolkit for useful quantum computing (von IBM)
- Weiterführende Quellen: [Awesome Quantum Software](https://github.com/qosf/awesome-quantum-software) | [Open-Source Quantum Software Projects](https://quantumcomputingreport.com/tools/) | [qosf](https://qosf.org/project_list/)

## Kostenlose Alternativen

- Atlassian **Jira**
	- Web/Self-Hosted: **[OpenProject](https://www.openproject.org/)** \[via [docker](https://www.openproject.org/docs/installation-and-operations/installation/docker/)\] | **[GitLab](https://about.gitlab.com/install/)**
	- Cloud: **[YouTrack](https://www.jetbrains.com/youtrack/)** | **[GitLab](https://about.gitlab.com/pricing/)**
- Atlassian **Confluence**
	- Web/Self-Hosted: **[XWiki](https://www.xwiki.org)** | **[BlueSpice](https://bluespice.com/products/bluespice-free/)**
	- Cloud: **[MyXWiki.org](https://myxwiki.org)**
- Atlassian **Bitbucket**
	- Web/Self-Hosted: **[GitLab](https://about.gitlab.com/install/)**
	- Cloud: **[GitLab](https://about.gitlab.com/pricing/)**
- Atlassian **Bamboo**
	- Web/Self-Hosted: **[GitLab](https://about.gitlab.com/install/)**
	- Cloud: **[GitLab](https://about.gitlab.com/pricing/)**
- Atlassian **FishEye**
	- Web/Self-Hosted: **[Sourcegraph](https://sourcegraph.com/search)** | [OpenGrok](https://oracle.GitHub.io/opengrok/)
- Atlassian **Crucible**
	- Web/Self-Hosted: [**Gerrit** Code Review](https://www.gerritcodereview.com/)
	- Cloud: [JetBrains **Space**](https://www.jetbrains.com/space/) | [Codeball.ai](https://codeball.ai/) | [Amazon CodeGuru](https://aws.amazon.com/de/codeguru/)
- Atlassian **WhiteSource** → heute: **Mend**.io
	- ToDo (Diverse! Kuratierte kostenlose Empfehlung offen. Cloud: [JFrog XRay](https://jfrog.com/xray/)?)
- JFrog **Artifactory** / Sonatype **Nexus**
	- = Software-Artifact-Repositories! Beide Vorreiter bieten auch kostenlose Varianten:
	- Web/Self-Hosted: [Sonatype **Nexus**](https://de.sonatype.com/products/repository-oss-download) (OSS-Version), Inedo **[ProGet](https://inedo.com/proget/download)** (Free Version)
	- Cloud: [JFrog **Artifactory**](https://jfrog.com/artifactory/) (free: 2GB, 5 Users)
- **VMware** Workstation
	- Desktop: **[VirtualBox](https://www.virtualbox.org/)** \[**choco install virtualbox**\] | **[Hyper-V](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/quick-create-virtual-machine)**
- **VMware vSphere**
	- **[Proxmox VE](https://www.proxmox.com/proxmox-ve)** (Linux-only)
- Altova **XMLSpy** / **Liquid Studio**
	- (Leider gibt es hierfür kaum adäquaten FOSS-Ersatz)
	- XML-Aspekte
		- Desktop: **[XML Notepad](https://microsoft.GitHub.io/XmlNotepad/)**
		- Cloud: **[XmlGrid.net](https://xmlgrid.net/)** | **[CodeDestine XML Editor](https://codedestine-xmleditor.netlify.app/)**
	- JSON-Aspekte:
		- Desktop: **[DbGate](https://dbgate.org)** \[**choco install dbgate.portable**\] | [**Datroit** JSON Viewer](https://dadroit.com/) | **[JSONedit](https://tomeko.net/software/JSONedit/)**
		- Browser Plugins: **[JSON Viewer Pro](https://github.com/rbrahul/Awesome-JSON-Viewer)** (Best-in-class JSON Visualisierung)
		- Cloud: **[Online JSON Viewer](http://jsonviewer.stack.hu/)**
		- Visualize the schema lurking behind your JSON documents in UML: **[JSON discoverer](http://som-research.uoc.edu/tools/jsonDiscoverer/#/)**
- **Unity / [](http://jsonviewer.stack.hu/)** Epic Games **Unreal Engine**
	- Royalty-free, Open Source: **[Godot](https://godotengine.org/)** \[**choco install godot**\]
		- (Eher [nicht verwenden](https://hackaday.com/2022/01/10/open-3d-engine-amazons-old-clothes-or-a-game-engine-to-truly-get-excited-about/): [O3DE](https://www.o3de.org/) = Open 3D Engine, basierend auf AWS Lumberyard bzw. CryEngine)
	- (Licensing above Threshold: [**Unity** Student](https://store.unity.com/#plans-individual), but [beware its licensing](https://unity3d.com/unity/activation/personal) and EULA)
	- (Royalties above Threshold: Epic Games [**Unreal** Standard License](https://www.unrealengine.com))
	- **Konsolen?**: [Godot vs. **Consoles**](https://godotengine.org/article/godot-consoles-all-you-need-know/) (gilt auch für Unity oder Unreal, bspw. „It is a common misconception that you can download a game engine and start using it to develop for consoles without previously being approved by the console manufacturer.“)
	- **Steam?** Auch **[Godot](https://store.steampowered.com/app/404790/Godot_Engine/)** per **[GodotSteam](https://godotsteam.com/)**. (Disclaimer: [Unity wurde zur beliebtesten Game Engine für Steam](https://www.gamedeveloper.com/business/game-engines-on-steam-the-definitive-breakdown), Stand 2020.)

## Bonus: Studentisches Start-Up (Software-Entwicklung)

- IT-Infrastruktur
	- Small Business Linux Server? **[KeyHelp](https://www.keyhelp.de/)** für Linux (Deutsch und kostenlos, aber kein Open-Source)
	- Virtuelle Maschinen? **[Proxmox VE](https://www.proxmox.com/proxmox-ve)**, eine Open-Source-Plattform für Enterprise-Virtualisierung
	- Kubernetes? Red Hat **[OKD](https://www.okd.io/)** (OpenShift-basiert) | Rancher **[RKE](https://rancher.com/products/rke)** (Pure-Container-basiert, über [RancherOS](https://github.com/rancher/os)) \[**choco install rke**\]
	- Firewall? **[OPNsense](https://opnsense.org/)**
	- VPN? **[WireGuard](https://www.wireguard.com/)** \[**choco install wireguard**\], statt IPsec oder OpenVPN
	- Softwareverteilung? **[Opsi](https://www.opsi.org/de/)**
	- Active Directory? **[Samba](https://www.samba.org/)**
	- Passwort Manager? **[Vaultwarden](https://github.com/dani-garcia/vaultwarden)** \[via docker\]
- Querschnitt
	- Doodle/Terminumfragen
		- Cloud: **[nuudel](https://nuudel.digitalcourage.de/)** | **[fragab](https://fragab.com/)**
		- Web/Self-Hosted: **[Framadate](https://framagit.org/framasoft/framadate/framadate)**
	- Chat? **[RocketChat](https://de.rocket.chat/install)** \[**choco install rocketchat**\]\[[Cloud](https://cloud.rocket.chat/)\]
	- Video Conference? **[Jitsi](https://jitsi.org/)** \[**choco install jitsi**\]\[[Cloud](https://meet.jit.si/)\]
		- Alternative: **[Nextcloud Talk](https://nextcloud.com/talk/)**, als FOSS via [NextCloud Server](https://nextcloud.com/install/) → Müsste jemand mal für mich ausprobieren…
	- DMS/CMS? [**Alfresco** Community Edition](https://www.alfresco.com/products/community/download)
	- Workflow Management / Case Management? **[flowable](https://www.flowable.com/open-source)** (welches ggb. Activiti oder Camunda zu bevorzugen ist)
- Vertrieb & Marketing
	- CRM? **[SuiteCRM](https://suitecrm.com/download/)** | Cloud-Alternative: [**Zoho CRM** free plan](https://www.zoho.com/crm/signup.html?plan=free&src=crmpricing), kostenlos für drei Nutzer
	- Newsletter / E-Mail Marketing: **[SendInBlue](https://de.sendinblue.com/)** | **[SendGrid](https://sendgrid.com/)**
	- Online Marketing: **[marketplan.io](https://marketplan.io/)**, **[predis.ai](https://predis.ai/)**
	- Online Lead Generation: **[apiway.ai](https://apiway.ai/)**
	- e-Commerce: Open-Source **[WooCommerce](https://github.com/woocommerce/woocommerce)** über [WordPress](https://wordpress.org/)
- Produktion & Softwareentwicklung
	- SW-Versionsverwaltung: **[GitLab](https://about.gitlab.com/install/)**
	- SW-Artefakt-Repository: [Sonatype **Nexus**](https://de.sonatype.com/products/repository-oss-download) (OSS-Version)
- Kundendienst & Support
	- Ticketing: [Zammad](https://zammad.org)
- Administration & Finanzen
	- Geschaftsbrief: [DIN 5008](https://leonrenner.com/din-5008-geschaeftsbrief-regeln-fuer-den-aufbau-nach-norm/)
	- HR? **[ConnecTeam](https://connecteam.com/)** (Cloud) | [**TimeOff**.Management](https://github.com/timeoff-management/timeoff-management-application) (FOSS, Web/Self-Hosted) | List of [Best Open-Source HRMS](https://wperp.com/68603/best-open-source-hrms/)
- Enterprise One-Stop-Shop
	- Enterprise Suite: **[WikiSuite](https://wikisuite.org/)** für Linux („Not-so-Small Business Linux Server – on Steroids“, FOSS), substituiert Ihnen nicht nur KeyHelp (SMB Linux Server) sondern auch NextCloud (Groupware-Bedürfnisse) und Chat und VidConf sowie weitere der obigen Einzel-Empfehlungen in einem großen Open-Source-Software-Bündel

Bonusliste:

- Weiterführende Quellen: [Awesome Selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted)
- Kostenlose AWS-Budgets benötigt für ein Start-Up? **[AWS Activate](https://aws.amazon.com/de/activate/)**
- Niedrigpreis-Logo für Start-Ups? (€:) [logogeist.de](https://www.logogeist.de/pricing)

## Appendix: App Recommendations & Repos

- [**Chocolatey** Packages](https://community.chocolatey.org/packages) for Windows
- **[GetApp](https://www.getapp.com/)**
- **[Docker Hub](https://hub.docker.com/search?q=)**
- **[ArtifactHub](https://artifacthub.io/)**: Explore Helm charts from numerous public repositories
- [Snappy](https://snapcraft.io/) for Linux
- [Flatpak Flathub](https://flathub.org/apps) for Linux
- [Homebrew](https://brew.sh/) for macOS
- **[Libhunt](https://www.libhunt.com/)**
- **[DB-Engines](https://db-engines.com/en/ranking)**
- [Project Awesome](https://project-awesome.org/) | [Awesome Awesomeness](https://github.com/bayandin/awesome-awesomeness) | [Track Awesome List Updates Daily](https://www.trackawesomelist.com/)
- Lesen Sie auch [freeCodeCamp **How to Choose a Tech Career** in 2022](https://www.freecodecamp.org/news/how-to-choose-a-tech-career/) mit einem Mapping von Werkzeugen auf diverse Job-Profile
- [Liste von **Zapier**-kompatiblen Apps](https://zapier.com/apps)
- **[FutureTools](https://www.futuretools.io)**
- Windows: [Awesome **Windows**](https://github.com/thechampagne/awesome-windows)
- Mac: [Awesome **Mac**](https://github.com/jaywcjlove/awesome-mac)

## Appendix: More Free Student Stuff

- [GitHub Student Developer Pack](https://education.github.com/pack)
- [discount-for-student-dev](https://github.com/AchoArnold/discount-for-student-dev)
- [A-to-Z-Resources-for-Students](https://github.com/dipakkr/A-to-Z-Resources-for-Students)

## Footer

### Future Work

I plan to translate this awesome list from German into English at some point.

### Contribute

What did I miss? Anything you recommend?

Contributions are most welcome, please adhere to the contribution guidelines and ensure your pull request adheres to the following guidelines:

- Make an individual pull request for each suggestion.
- Keep descriptions short and simple.
- Check your spelling and grammar.
- Make sure your text editor is set to remove trailing whitespace.
- Try to make your Pull request and title as descriptive as possible.
- New categories or improvements to the existing categorization are welcome.

Thank you for your suggestions!

### Backers

Thank you to all our supporters! 🙏

_Please, consider supporting my work as a lot of effort takes place to generate this list! Thanks a lot._

[![Donate via PayPal](https://img.shields.io/badge/Donate-PayPal-0070BA?style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/donate/?hosted_button_id=QTDJ2JA58ZM9L)

[![Support on Ko‑fi](https://img.shields.io/badge/Support-Ko–fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/cyberlytics)

[![Buy Me A Coffee!](https://img.shields.io/badge/buy_me_a_coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/cyberpetaneuron)

### License

[![Creative Commons License](http://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

This work is licensed under Creative Commons [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/) .
