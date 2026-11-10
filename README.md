# PROJECT: ORACLOPÉDIA
## The official living encyclopedia of the Oracle Red Bull Racing Empire

You are a senior full-stack developer, UI/UX designer and AI integration engineer. Your task is to build a complete, functional web application named **Oraclopédia**, a French-language encyclopedia documenting the entire fictional universe of Pax Historia, particularly the history, institutions, territories, personalities, technologies and society of the Oracle Red Bull Racing Empire (ORBR).

This must be a real, usable application, not a static mockup or a simple landing page.

The application must be developed using **TypeScript and TSX**, with a modern web frontend.

---

# 1. CORE CONCEPT

Oraclopédia is essentially a fictional equivalent of Wikipedia.

It contains articles about everything that exists in the Pax Historia universe:

- Historical events
- Historical periods
- Countries and territories
- Cities and settlements
- Political institutions
- Governments and administrations
- Political figures
- Imperial families
- Military organizations
- Wars and diplomatic relations
- Companies and economic organizations
- Technologies and inventions
- Scientific discoveries
- Religion and philosophy
- Education
- Culture and literature
- Formula 1 teams, drivers and championships
- Infrastructure and public services
- Important documents and laws

The encyclopedia must continuously evolve as new events happen in the campaign.

## THE MOST IMPORTANT FEATURE: AI-POWERED ARTICLE MANAGEMENT

I want to manually provide new historical events to an AI chatbot integrated into the application.

For example, I might paste:

"On 12 September 1453, Emperor Max I inaugurated a new university in RedBullOpolis. The institution was named Oracle Imperial University and specializes in engineering, medicine and political sciences."

The AI must then:

1. Read and understand the submitted event.
2. Extract all relevant historical information.
3. Identify existing articles that are affected.
4. Determine whether new articles are necessary.
5. Generate new articles when appropriate.
6. Update existing articles with the new information.
7. Update relevant chronological timelines.
8. Establish connections between related articles.
9. Preserve all previously established historical information.
10. Present its proposed modifications for my approval.

For example, this event could result in:
- A new article about Oracle Imperial University.
- An update to the article about RedBullOpolis.
- An update to the article about Max I.
- An update to the article about higher education in the Empire.
- An addition to the timeline of 1453.

**The AI must never automatically publish modifications without my approval.**

I want a review interface where I can inspect, edit, approve or reject each proposed modification.

---

# 2. AI CHATBOT — THE HISTORICAL EDITOR

Create a dedicated AI assistant called:

**L'Archiviste d'Oraclopédia**

It must be accessible through a chatbot interface.

Its primary purpose is to transform manually submitted campaign events into structured encyclopedia content.

### Chatbot interface

The interface should contain:
- A large message history.
- A text input area.
- A button to submit new historical information.
- A button to clear the current conversation.
- A processing indicator.
- A way to inspect the articles affected by the submitted event.

I must be able to paste long texts containing several events, reports, biographies or historical developments.

The chatbot must understand French naturally, including informal writing, incomplete sentences, spelling mistakes and complex historical descriptions.

### AI workflow

The AI must follow this workflow:

**STEP 1 — ANALYSIS**

Analyze the submitted information and identify:
- Dates
- Locations
- People
- Organizations
- Political decisions
- Historical events
- Technologies
- Economic developments
- Relationships between entities

**STEP 2 — KNOWLEDGE RETRIEVAL**

Search the existing encyclopedia for relevant articles.

The AI must retrieve existing information before creating or modifying anything.

**STEP 3 — ARTICLE GENERATION**

Determine which articles need to be created and which need to be updated.

Use an encyclopedia writing style:
- Neutral
- Factual
- Historical
- Detailed
- Well structured
- Written in French

Avoid conversational language, personal opinions and unnecessary storytelling.

**STEP 4 — CONSISTENCY CHECK**

Check whether the new information contradicts existing articles.

If contradictions are detected:
- Highlight them.
- Explain the conflicting information.
- Do not silently overwrite existing historical facts.
- Ask me to resolve important ambiguities.

Distinguish between:
- Explicitly established facts.
- Uncertain information.
- Conflicting accounts.
- Inferences made by the AI.

Never invent dates, names, statistics, events or relationships.

**STEP 5 — REVIEW**

Display a list of proposed changes.

For each change, show:
- Article name.
- Action: CREATE or UPDATE.
- Previous content, if applicable.
- Proposed new content.
- Explanation of the modification.
- Source event supplied by the user.

Allow me to approve, edit or reject each change individually.

**STEP 6 — PUBLICATION**

Only after approval:
- Save the new articles.
- Update existing articles.
- Update relevant timelines.
- Update article relationships.
- Record the modification in the revision history.

---

# 3. ENCYCLOPEDIA STRUCTURE

Create a complete encyclopedia with the following main categories:

### Histoire
- Chronologie générale
- Grandes périodes historiques
- Guerres et conflits
- Traités et accords
- Révolutions et insurrections
- Événements majeurs

### Politique et institutions
- Empire Oracle Red Bull Racing
- Maison impériale
- Empereurs
- Dicastères
- Chancellerie
- Administrations provinciales
- Institutions judiciaires
- Réglementation
- Relations diplomatiques

### Géographie
- Pays
- Provinces
- Principautés
- Territoires
- Villes
- Capitales
- Régions
- Infrastructures géographiques

### Personnalités
- Famille impériale
- Chefs d'État
- Responsables politiques
- Diplomates
- Militaires
- Scientifiques
- Ingénieurs
- Artistes
- Sportifs
- Personnalités historiques

### Économie
- Monnaie
- Entreprises
- Commerce
- Industrie
- Agriculture
- Ressources naturelles
- Énergie
- Fiscalité
- Infrastructures économiques

### Sciences et technologies
- Électricité
- Énergie nucléaire
- Aviation
- Télécommunications
- Médecine
- Transports
- Inventions
- Innovations industrielles

### Société et culture
- Éducation
- Santé publique
- Religion et latifisme
- Littérature
- Théâtre
- Presse
- Architecture
- Traditions
- Vie quotidienne

### Sport automobile
- Formule 1
- Formule 2
- Formule 3
- Écuries
- Pilotes
- Circuits
- Grands Prix
- Championnats
- Règlements

Categories must be expandable and new subcategories must be possible.

---

# 4. ARTICLE DESIGN

Each encyclopedia article must have a professional Wikipedia-inspired layout.

An article should support:

- Title
- Subtitle or introductory description
- Main text
- Sections and subsections
- Images
- Captions
- Infoboxes
- Tables
- Chronological information
- Internal links to other articles
- External references, if manually supplied
- Categories
- Related articles
- Revision history

### Example: historical personality article

An article about Emperor Max I could contain:

**Max Ier**
*Empereur de l'Empire Oracle Red Bull Racing*

Infobox:
- Nom complet
- Naissance
- Fonction
- Début du règne
- Prédécesseur
- Successeur
- Épouse
- Enfants
- Nationalité
- Dynastie

Sections:
1. Origines
2. Ascension politique
3. Fondation de l'Empire
4. Règne impérial
5. Politique intérieure
6. Politique étrangère
7. Héritage historique

The AI should adapt the structure to the subject. A company, city, war or invention should have its own appropriate article format.

### Internal linking

Whenever an article mentions another entity that has its own encyclopedia entry, automatically create an internal hyperlink.

For example:

"Max Ier épousa [[Alice Bégon]] et eut un fils, [[Jos Louis Isack de la Bégoneraie Verstappen]]."

The links must lead to the corresponding articles.

If an article does not exist yet, the link can be displayed as an uncreated article, allowing me to create it later.

---

# 5. CHRONOLOGY SYSTEM

Create a dedicated chronological section.

It must allow navigation by:
- Year
- Month
- Day
- Historical period

Each event should have:
- Date
- Title
- Description
- Location
- Related personalities
- Related articles
- Event category

Example:

**1453**
- February: Introduction of the imperial education reforms.
- April: Antoine Derue patents his petroleum extraction system.
- May: Establishment of the new imperial transport regulations.
- July: Restoration of freedom of the press.

The chronology must be automatically updated whenever I approve a new event.

Support dates before and after the year 0 if necessary, and avoid assuming that every event has a precise date.

---

# 6. SEARCH ENGINE

Build a powerful search engine.

It should support:
- Article titles.
- Article content.
- Names and surnames.
- Historical dates.
- Locations.
- Organizations.
- Categories.
- Alternative spellings.

Add search suggestions and relevant results while typing.

Search should also recognize related concepts.

For example, searching "Leblanc" should return:
- Ernest Leblanc.
- Prime Leblanc.
- Stratégie Énergie 1453.
- Autorité de Régulation des Transports.

---

# 7. VISUAL DESIGN

The application must feel like a real, established encyclopedia.

Take inspiration from Wikipedia, Britannica and professional historical archives, but create an original identity for Oraclopédia.

### General appearance

- Clean and readable interface.
- Light background.
- Dark text.
- Restrained imperial red accents.
- Elegant typography.
- Clear article hierarchy.
- Well-designed infoboxes.
- Minimal unnecessary decoration.

### Header

Include:
- Oraclopédia logo.
- Search bar.
- Main navigation.
- Button to access the AI Archivist.
- User settings.

### Homepage

The homepage should contain:

1. A prominent search bar.
2. A welcome section introducing Oraclopédia.
3. Featured historical articles.
4. Recent historical events.
5. Recently updated articles.
6. Main encyclopedia categories.
7. A chronological overview.
8. An easy-to-access AI submission area.

### Article sidebar

On article pages, provide:
- Table of contents.
- Article categories.
- Related articles.
- Last modification date.

Make the entire application responsive for desktop, tablet and mobile.

---

# 8. TECHNICAL REQUIREMENTS

Use:
- TypeScript.
- TSX.
- React.
- A modern web application framework such as Next.js.
- Tailwind CSS or an equivalent styling solution.
- A structured database.
- A reliable AI integration layer.

Choose an appropriate database architecture. SQLite is acceptable for a local-first version; PostgreSQL is preferable if the application is deployed online.

### Data architecture

Do not store the entire encyclopedia in a single giant text file.

Create structured entities for:
- Articles
- Categories
- Historical events
- People
- Places
- Organizations
- Article relationships
- Article revisions
- AI submissions
- Pending changes

Each article should have a stable identifier independent of its title.

Support article redirects and title changes without breaking internal links.

### AI architecture

Create a modular AI service that can be connected to an LLM provider.

Do not hardcode an API key.

Use environment variables for credentials.

Provide a clear configuration page explaining how to connect the AI provider.

The AI must be able to:
- Search the database.
- Retrieve relevant articles.
- Generate structured article updates.
- Return proposed changes in a predictable format.
- Wait for approval before saving anything.

Use structured JSON outputs or an equivalent validated schema for article modifications.

### Persistence

All approved modifications must survive:
- Page reloads.
- Browser restarts.
- Application restarts.

Implement regular database backups or an export mechanism.

---

# 9. EDITORIAL INTEGRITY AND HISTORICAL CONSISTENCY

This is extremely important.

Oraclopédia documents a fictional alternate-history universe.

The AI must treat the user-provided Pax Historia lore as the authoritative historical source for the encyclopedia.

It must not replace fictional events with real-world historical events.

For example, if the user establishes that a fictional empire controls a territory, the encyclopedia must reflect that fictional reality.

However, the AI must never silently fill gaps with invented details.

It must preserve:
- Exact names.
- Exact dates.
- Established political titles.
- Established geographical terminology.
- Established institutional names.
- Historical relationships.
- Previously established statistics.

When the user supplies an update that changes an established fact, the AI must identify the change and ask whether it is a correction, a new development or a deliberate retcon.

Maintain a clear revision history so that earlier versions of articles can be inspected and restored.

---

# 10. ADMINISTRATION AND EXPORT

Create an administration interface allowing me to:

- Create articles manually.
- Edit articles manually.
- Delete articles with confirmation.
- Manage categories.
- Review AI proposals.
- Inspect revision history.
- Restore previous article versions.
- Manage redirects.
- Export the entire encyclopedia.
- Import previously exported data.

Support exporting articles in Markdown and JSON.

Also provide a full database backup.

---

# 11. IMPORTANT USER WORKFLOW

The application must make this process extremely simple:

1. I open Oraclopédia.
2. I click on "Archiviste IA".
3. I paste a new Pax Historia event or historical report.
4. The AI analyzes the text.
5. It searches the existing encyclopedia.
6. It proposes new articles and updates.
7. I inspect the proposed changes.
8. I approve or modify them.
9. The encyclopedia is updated.
10. The new information becomes searchable and appears in the relevant timelines.

I should not need to manually locate every article affected by a new event.

The AI should handle that work.

---

# 12. DEVELOPMENT AND DELIVERY

Build the complete application, not just a prototype.

Prioritize a working end-to-end implementation:
- Functional navigation.
- Working article pages.
- Search.
- Database persistence.
- Article editing.
- AI chatbot integration.
- AI-generated change proposals.
- Approval workflow.
- Revision history.
- Chronology.
- Export and import.

Include realistic sample articles based on the existing ORBR universe, but clearly distinguish those examples from the user's future submissions.

Do not fabricate additional historical events merely to populate the encyclopedia.

Provide:
1. The complete source code.
2. A clean and organized project structure.
3. A working setup guide.
4. Installation instructions.
5. Database configuration instructions.
6. AI provider configuration instructions.
7. Instructions for running the application locally.
8. Deployment instructions.

Do not stop after creating the homepage. Implement the actual application and test the entire workflow, especially the process of submitting an event, generating article modifications, approving them and seeing the updated articles.

**FINAL OBJECTIVE: Oraclopédia must become the central, continuously updated historical encyclopedia of the Pax Historia universe, with me acting as its chief editor and the AI acting as its historical researcher and assistant editor.**
For first sources go to this repo where you can find the pdf files with the first batch of lore : https://github.com/glasco90/new-pdf-lore.git
