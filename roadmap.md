🗓 Project Roadmap (1.5 Weeks / 10 Days)


| **Day**     | **Milestone**                        | **Tasks / Deliverables**                                                                                                                                             | **Tools / Tech**                        |           |                            |
| ----------- | ------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- | --------- | -------------------------- |
| **Day 1**   | **Setup & Data Prep**                | - Create Git repo & folder structure<br>- Install dependencies (Whisper / Google STT, LangChain, SpaCy, etc.)<br>- Collect sample meeting audio/video files          | Python, Whisper / Google STT, PyDub     |           |                            |
| **Day 2–3** | **Speech-to-Text Module**            | - Implement audio preprocessing (PyDub: trimming, splitting, format conversion)<br>- Integrate Whisper API for transcription<br>- Store raw + transcribed text in DB | Whisper API, PyDub, FastAPI, PostgreSQL |           |                            |
| **Day 4**   | **Summarization Pipeline**           | - Use LangChain with GPT/Mistral for meeting summarization<br>- Design chunking + summarization flow (map-reduce)<br>- Output key topics & discussion summary        | LangChain, GPT-4 / Llama-3              |           |                            |
| **Day 5**   | **Action Item & Keyword Extraction** | - Build NER pipeline (SpaCy/HF Transformers)<br>- Add prompt-based extraction using LLMs<br>- Format results as “Task                                                | Owner                                   | Deadline” | SpaCy, GPT-4, Transformers |
| **Day 6**   | **Sentiment & Emotion Analysis**     | - Apply VADER / HuggingFace sentiment models<br>- Generate sentiment score & tone insights<br>- Save outputs in structured format                                    | VADER, HuggingFace                      |           |                            |
| **Day 7–8** | **Dashboard & Visualization**        | - Build Streamlit dashboard:<br> • Meeting summary viewer<br> • Sentiment bar/pie chart<br> • Action items table<br> • Speaker talk-time / topic frequency graph     | Streamlit, Plotly, Matplotlib           |           |                            |
| **Day 9**   | **Integration & Export**             | - Add export functions: Notion / Gmail / Slack APIs<br>- Automate summary sending post-meeting<br>- Integrate with Zoom/MS Teams (mock or real)                      | Gmail API, Slack API, FastAPI           |           |                            |
| **Day 10**  | **Testing & Final Demo**             | - End-to-end pipeline test<br>- Fix bugs & UI polish<br>- Record demo video and documentation                                                                        | pytest, Streamlit, Markdown docs        |           |                            |




🚀 Deliverables at End of Week 1.5

✅ Functional transcription → summary → sentiment → dashboard pipeline

✅ Action item extraction (Owner, Deadline, Task)

✅ Export integration (e.g., Email/Slack/Notion)

✅ Streamlit dashboard demo



Person A — “Core AI & Meeting Intelligence”

Focuses on the intelligence side (summary, action items, sentiment), end-to-end:

| **Scope**                       | **Tasks (Full-Stack)**                                                                                                                    | **Learning Areas**                                |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------- |
| 🧠 **Summarization & Insights** | - Implement LangChain + GPT/Mistral summarizer<br>- Design summary endpoint in FastAPI<br>- Build Streamlit “Summary Viewer” UI card      | Prompting, LLM APIs, LangChain, API creation      |
| 📋 **Action Item Extraction**   | - Implement SpaCy/NER extraction<br>- Serve via `/extract_action_items` endpoint<br>- Create Streamlit task table (Task, Owner, Deadline) | NER, NLP, JSON formatting, data visualization     |
| 💬 **Sentiment Analysis**       | - Integrate VADER / HuggingFace sentiment<br>- Add sentiment summary API<br>- Build Pie/Bar visualization                                 | NLP model integration, plotting, UI interactivity |



Person B — “Speech & Integration Systems”

Focuses on the data & delivery side (audio → text → dashboard export), end-to-end:

| **Scope**                      | **Tasks (Full-Stack)**                                                                                              | **Learning Areas**                                   |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| 🎧 **Speech-to-Text Pipeline** | - Implement Whisper or Google STT<br>- Preprocess audio (PyDub)<br>- Create `/transcribe` API + Streamlit upload UI | Audio processing, Whisper API, REST API              |
| 📊 **Analytics Dashboard**     | - Build talk-time, topic frequency charts (Matplotlib/Plotly)<br>- Design overall dashboard layout                  | Data visualization, chart design, layout structuring |
| 🚀 **Integration & Export**    | - Implement export (Gmail/Slack/Notion)<br>- Build simple “Export Summary” frontend button                          | API authentication, web integration, automation      |


