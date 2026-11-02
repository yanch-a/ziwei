# Lingjing Shensuo · Zi Wei Dou Shu & AI Study Platform

[中文介绍](README.md) | English

> Connecting traditional chart knowledge, personal experience, and AI conversation.

**Lingjing Shensuo (灵境深索)** combines Zi Wei Dou Shu chart calculations, specialist knowledge dictionaries, and large-language-model interpretation. The system identifies what a user is asking, calculates the relevant chart, and prepares an interpretation using school-specific rules, domain knowledge, and personal context. Record management, interactive chart views, life histories, and learning resources support an ongoing workflow from visual exploration to follow-up questions.

Developed by **yanch**, the project serves enthusiasts, learners of traditional Chinese culture, and users who maintain chart collections for ongoing case studies.

## Live Demo

- **Demo URL:** [http://test.ychos.cn:7707/](http://test.ychos.cn:7707/)
- **Username:** `yanch`
- **Password:** `123456`

![Lingjing Shensuo San He chart](images/02-sanhe-chart.jpg)

## Distinctive Features

### Programmatic Chart Calculations Inform AI Interpretation

The project's own software calculates natal charts and dynamic charts for major periods, annual periods, and other time layers. Structured results feed into prompt construction, giving the AI concrete star, palace, and transformation data to discuss. Users can consult the visual chart alongside the explanation.

### Separate Analytical Approaches for San He and Four Transformations

San He and Four Transformations use distinct prompt and data-building logic. San He incorporates star combinations, star strength, and the Three Directions and Four Positions. Four Transformations incorporates natal transformations, the Lai Yin palace, inward and outward self-transformations, palace-stem flying transformations, and Fa Xiang Hui Gui relationships, with corresponding meaning dictionaries. San He, Flying Star, and Four Transformations views make these relationships available for visual study.

### Questions Drive the Analysis Context

The conversation service distinguishes chart creation, knowledge questions, chart analysis, and follow-ups, then extracts relevant years, major periods, palaces, and analytical schools. A career question about a particular year can trigger calculation of that annual chart and preparation of relevant palace and transformation data. Follow-ups can inherit earlier analysis parameters, while the routing workflow supports clarification when required information is missing.

### Life Histories Contribute Relevant Personal Context

Personal chart records bring user-supplied experiences into the discussion. The system can select life-history categories associated with the relevant palace, summarize key events, and include them alongside chart information. A career-related discussion, for example, can draw on associated career experiences supplied by the user.

### Knowledge Questions Use Retrieved Reference Material

The knowledge-question workflow integrates vector retrieval from a Zi Wei Dou Shu knowledge base and uses retrieved material as answer context. Together with specialist dictionaries for stars, palaces, and transformations, this provides a maintainable foundation of domain material for learning and analysis.

### Engineering Tools Support Domain Data Development

The project also includes annotation and batch-processing modules for natal Four Transformations, flying transformations, major-period palace overlays, and Fa Xiang Hui Gui. These tools prepare samples, retain analytical explanations and conclusions, and export JSONL data for subsequent training and validation work.

These features describe implementations found in the current source code. Desktop and mobile screenshots appear below; availability depends on the application version.

## Desktop Features and Screenshots

### 1. Chart Record Management

Manage names, gender, Gregorian and lunar birth information, groups, and notes in one place. Search by name or notes, browse groups such as family, friends, classmates, colleagues, and clients, and access record import, export, and chart generation tools.

![Chart records and groups](images/01-chart-library.jpg)

### 2. Interactive Chart Exploration

Create charts using Gregorian or lunar dates, or use the Four Pillars reverse lookup to find matching birth dates. Switch between San He, Flying Star, and Four Transformations views to explore the twelve palaces and star placements. Major-period and annual, monthly, daily, and hourly selectors support exploration across different time layers. Charts can also be saved as images.

The San He view appears at the top of this page. The following screenshots show the other two perspectives.

**Flying Star view:** Displays key stars, transformation markers, and major-period palace information for studying palace relationships.

![Flying Star chart](images/03-feixing-chart.jpg)

**Four Transformations view:** Uses colored markers and connecting lines to make transformation relationships easier to follow.

![Four Transformations chart and relationship lines](images/04-sihua-chart.jpg)

### 3. AI-Assisted Interpretation

The interpretation menu provides entry points for natal, major-period, and annual analysis. Users can select an individual palace or open the natal-chart interpretation. Streaming endpoints allow generated content to appear progressively.

In the captured desktop version, **monthly, daily, and hourly AI interpretation are marked as unavailable**. These AI entry points are separate from the chart's time-selection controls.

![AI interpretation types and palace selection](images/05-ai-analysis.jpg)

### 4. Personal Charts and Life Histories

Record experiences under categories such as education, career, relationships, and family changes, with room for custom entries. The project supports including these records as background for AI conversations, connecting chart discussions with experiences supplied by the user.

![Personal chart and life-history form](images/06-life-history.jpg)

### 5. AI Conversations

Ask the built-in assistant about Zi Wei Dou Shu concepts directly, or select a chart for a contextual discussion. The interface includes new conversations, conversation history, chart switching and viewing, access to life histories, and several visual themes.

![Zi Wei Dou Shu AI assistant](images/07-ai-chat.jpg)

### 6. Learning Resources

The learning section organizes material into software guidance, Zi Wei Dou Shu terminology, notable figures, and advanced study. Category browsing and content search help users find reference material while studying charts and concepts.

![Zi Wei Dou Shu learning resources](images/08-knowledge-center.jpg)

## Mobile · Chart Exploration and AI Study on the Go

The mobile application brings chart exploration, record management, AI interpretation, and learning resources to the phone. Bottom navigation connects charts, Lingjing conversations, help, and the personal center, supporting a continuous workflow from selecting a record to reading an interpretation and asking follow-up questions. The following images are the project's supplied iOS screenshots.

### 1. San He and Four Transformations on a Phone

The portrait layout retains all twelve palaces, star information, transformation markers, and relationship lines. Time-selection rows cover major periods, annual periods, and other layers, alongside controls for Flying Star, San He, and Four Transformations views and quick chart creation.

| San He chart | Four Transformations chart |
| --- | --- |
| <img src="images/mobile/sanhe.png" alt="iOS San He chart" width="280" /> | <img src="images/mobile/sihua.png" alt="iOS Four Transformations chart" width="280" /> |

### 2. Interpretation by Year and Palace

The AI interpretation menu organizes natal, major-period, and annual analysis, with year and target-palace selection. Generated content appears progressively in a reading panel over the chart, with controls to stop generation and share results.

| Analysis selection | Interpretation reader |
| --- | --- |
| <img src="images/mobile/ai.png" alt="iOS annual and palace analysis selection" width="280" /> | <img src="images/mobile/jx.png" alt="iOS AI interpretation reader" width="280" /> |

### 3. Ongoing Conversations About a Selected Chart

The Lingjing conversation page provides chart selection, conversation history, and new conversations. Users can ask follow-up questions about palaces, star combinations, and personal topics. The example shows a description of the identified request and a chart overview, helping users check the context of the discussion.

| Conversation entry | Chart discussion |
| --- | --- |
| <img src="images/mobile/chat.png" alt="iOS AI assistant and chart selection" width="280" /> | <img src="images/mobile/chat2.png" alt="iOS chart discussion and analysis context" width="280" /> |

### 4. Knowledge Retrieval and Learning Resources

Knowledge questions can incorporate retrieved Zi Wei Dou Shu material; the screenshot shows relevant reference excerpts. The help center organizes searchable articles into software guidance, terminology, notable figures, and other categories for consulting concepts and instructions while studying.

| Knowledge questions and retrieved excerpts | Help center |
| --- | --- |
| <img src="images/mobile/kep.png" alt="iOS knowledge questions and retrieved references" width="280" /> | <img src="images/mobile/help.jpg" alt="iOS help and learning categories" width="280" /> |

### 5. Chart Records and Personal Center

The record list provides name or note search, group filtering, and controls to add, edit, delete, and open charts. The personal center displays membership tier, status, validity, and invitation information for reviewing account and service details.

| Chart records | Personal center |
| --- | --- |
| <img src="images/mobile/personList.png" alt="iOS chart record search and management" width="280" /> | <img src="images/mobile/me.png" alt="iOS personal center and membership information" width="280" /> |

## Typical Workflow

1. Create or import a chart record, then organize birth details, groups, and notes.
2. Open the chart and explore its palaces and time layers through the available views.
3. Add relevant life-history entries to provide personal context.
4. Choose an interpretation entry point or continue discussing the chart in AI chat.
5. Review concepts in the learning section, save chart images, and build a collection of cases.

## Technical Overview

| Layer | Technologies and responsibilities |
| --- | --- |
| User interface and desktop | Vue 3, Element Plus, and Electron for record management, chart visualization, and AI chat |
| Mobile | uni-app and Vue 3 for phone-based charts, AI conversations, help, and personal-center pages |
| Business backend | Java, Spring Boot, and MyBatis-Plus for chart records, life histories, sessions, and analysis APIs |
| AI services | Lemon AI and Spring AI for model integration and analysis services, with SSE streaming responses |
| Domain data | Dictionaries for stars, palaces, and Four Transformations, plus modules for prompts and model data management |

## Project Information

- **Name:** Lingjing Shensuo (灵境深索)
- **Developer:** yanch
