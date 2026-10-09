# 英语视频学习模式

## Watch and ask

The user watches an English video with meeting recording/transcription and types unfamiliar terms or sentences into the chat. Stay quiet between questions; do not interrupt playback with unsolicited corrections, vocabulary lists, or forced speaking exercises. Ask for a video link/title only when missing context materially prevents an answer; keep it as source metadata when supplied. Use the current selected recording Page or explicit session reference, not a hardcoded Page ID or an unrelated old meeting.

For each question, retrieve the available source transcript before explaining its contextual meaning. Discover `read_page_transcript` or the environment's equivalent and obey its schema and Page guidance. A speaker label such as “You” may include playback audio: do not identify video speech as the user's English solely from that label.

Live/preliminary text may be incomplete or have recognition errors. Refresh it when the question concerns new speech. Follow final transcript continuation when needed; exhaust it before summarizing the whole video. Never infer that omitted material was not discussed. If the term cannot be located, ask for the subtitle sentence or time point; offer only a clearly labeled general explanation meanwhile. If transcript access is unavailable, work from the user's provided sentence/subtitles and state the context limitation. Do not imply that you watched unseen frames or heard audio that no tool supplied.

Keep answers short enough for watching to continue:

- English term and its Chinese meaning in this passage.
- What the surrounding claim means, using plain Chinese and a concrete example when helpful.
- Recognition correction or ambiguity, if it changes the meaning. Preserve the original recognized text separately from the checked term.

Check unfamiliar technical claims or current product details against primary sources when needed; keep source links. Distinguish what the video claims, a checked definition, and your interpretation. Do not invent a user's reaction or connect every term to a creator use case; include creator relevance only when supported or requested.

Quietly collect the terms the user actually asks about and any expressions they explicitly request to record. Keep the question, relevant source sentence/available time point, explanation, and the user's own expressed understanding. No automatic exhaustive vocabulary harvesting. “现在记下来” requests an immediate authorized Obsidian write; otherwise batch the write at closing. This learning record is not a global-memory update.

## Optional speaking bridge

If the user chooses to explain or retell a passage in English, let them finish, then give selective feedback on both meaning and expression. Store only their own speech in the speaking-practice transcript and feedback. Do not require retelling to complete a video session and do not count video playback words or duration as the user's speaking statistics.

## Learning content: English first, AI context retained

During playback, keep explanations short; expand them when closing and saving. Always capture asked-about terms. At closing, also select a small number of useful spoken expressions and AI-related concepts actually present in the available source. Label them as agent-selected suggestions, distinct from user questions. Do not harvest every unfamiliar word or invent reactions.

For each focal word or phrase, record: base form and part of speech; form used in the source; contextual Chinese meaning; a short source sentence and its meaning; the term's role/use in that sentence; one or two useful collocations; a simple additional example in a different scenario. Add pronunciation guidance or confusing meanings only when useful. Label generated examples as examples, not quotations.

Keep useful spoken expressions as reusable chunks: expression, Chinese meaning, appropriate situation, and one example. Keep detailed explanations in the session note and concise entries in the video-learning vocabulary notebook; use links instead of duplicating full explanations.

AI learning has a separate part. Extract concepts needed to understand the video's claims, tasks, and human-agent collaboration. Distinguish AI concepts/capabilities, software-development terms, and general workplace language (for example, PR and regressions are not AI-specific terms). For each selected concept give: English/Chinese name, plain explanation, how it appears in the video, and its significance or remaining uncertainty. Check unfamiliar technical claims and current product capabilities against primary sources when necessary. Separate video claims, independently verified facts, and interpretation; do not treat a demo as capability verification. For non-AI videos adapt this part to relevant subject concepts or omit it.

## Closing quiz and evidence-based feedback

When the user ends learning, normally offer and begin a brief quiz before final feedback and archiving. Ask one question per turn and wait for the actual answer; do not provide the answer or a leading hint in the question. Typed Chinese answers are accepted for meaning and concept checks; English output is required only when assessing English usage. Playback remains uninterrupted until closing.

Questions focus on vocabulary, with fewer AI questions: typically three or four vocabulary/expression questions and zero or one AI/content question, reduced for small sessions or limited time. These are defaults, not quotas. Sample within the session's relevant material; prioritize explicitly asked terms and known confusions. Mix contextual meaning, part-of-speech/use when informative, application to a new situation, and short completion/production tasks. Do not ask obscure facts, exact timestamps, or untaught concepts. Each question checks a clear learning target.

After each answer, give brief feedback, the missing distinction if any, and an optional retry when useful. Record the question, user's answer, whether a hint was used, and the specific evidence. Distinguish meaning comprehension from English production; a Chinese explanation cannot establish English usage proficiency. Use local outcomes such as `本题独立答对`, `提示后答对`, `本题仍有混淆`, and `未测`, rather than declaring lasting mastery after one correct answer. Do not infer pronunciation or listening accuracy from typed answers alone.

The user can skip or stop the quiz and still request archiving. Save completed responses and mark the rest untested; do not fabricate understanding, progress, or difficulties from explanations alone. If the user says only to stop, stop without continuing a quiz or archive. A request for direct saving takes precedence over the default quiz.

## Save the session to Obsidian

When the user requests closing and archiving, save within the established learning system after the brief quiz or its explicit skip. Session-specific write authorization persists; do not ask again for the same destination. If only a summary is requested, answer in chat.

Locate and verify the live Vault before writing. Use the user’s configured Vault and language-learning parent folder; inspect existing structure or ask for the location if it cannot be established. Preserve existing notes and indexes. Read [record schema](record-schema.md) for vocabulary columns and the speaking format.

Use sibling directories:

```text
语言学习/
├── 英语口语练习/       # existing speaking system with its own 单词本
└── 英文视频学习/
    ├── INDEX.md
    ├── YYYY-MM-DD 视频主题.md
    ├── 待办清单.md
    ├── 单词本/
    │   ├── INDEX.md
    │   └── YYYY-MM-DD.md
    ├── 对话记录/
    │   └── YYYY-MM-DD/
    │       ├── 对话记录.md
    │       └── 完整逐字稿.md
    └── 周复盘/
        ├── INDEX.md
        └── YYYYMMDD-MMDD.md
```

Do not nest video learning inside speaking practice. Keep separate vocabulary notebooks in each mode: `英文视频学习/单词本/` for video material and `英语口语练习/单词本/` for speaking material. Link across modes when useful, without copying every entry. Use newest-first indexes, one note per video session, and existing same-session notes instead of duplicates. Disambiguate different same-day videos naturally. Add links to both learning areas without rearranging unrelated sections.

The video note uses a familiar content → learning → feedback → next step → summary structure:

1. **本次内容**: source title/link, date, a small `这次学到了什么` overview, then `视频在讲什么`. Show the main claim and ordered segments. For demos, use task → assistant action → human feedback when helpful. Note missing title or limited coverage without fabricating metadata.
2. **学习情况**: watched/transcribed scope and source reliability where material; actual learning feelings only when expressed. No invented duration, speaking statistics, or mood tags.
3. **学习重点**: `AI 术语与功能理解` (or relevant subject concepts), `重点词汇`, `值得记的口语表达`, and `我的问题与答疑`. Link repeated explanations instead of restating them; preserve the actual user question and resolved confusion.
4. **本次反馈**: one concise evidence-based summary, then quiz question/answer/outcome/evidence or correction table. Group real difficulties and demonstrated progress using the speaking system's familiar headings where useful. If no quiz/output occurred, state `本次未回考` or `未测`; do not infer learning outcomes.
5. **后续练习**: unresolved questions and a small optional practice suggestion from the material. Distinguish suggested practice from user commitments.
6. **本次总结**: actual takeaways and expressed understanding, with links to vocabulary and the same-week review. Preserve creator ideas only when actually expressed; label proposed ideas separately from decisions.

Add asked-about reusable words/phrases to the video-learning vocabulary notebook and its index using the established vocabulary columns, linking to the video note. Selected additional entries should be few and clearly labeled as suggestions. Avoid duplicate word entries within the same session; retain technical detail in the video note. For the same word encountered again, link previous context and add only the new sense/use or quiz evidence rather than copying the full explanation.

Every authorized video-session archive also creates or updates its own `对话记录/日期/对话记录.md`, vocabulary/index, main index, relevant pending items in `待办清单.md`, and same-week material-collection note. The dialogue record follows Chinese summary → learning situation → actual questions and answers → evidence-based feedback → next steps → closing summary. Preserve actual messages separately from reconstructed Q&A; label reconstructions and unavailable full transcripts honestly. For multiple same-day sessions, give each session a stable topic or recording identifier. Keep separate sections in the daily dialogue record and raw-transcript file, or use topic subfolders when the existing layout does so; retain earlier text. When refreshing a preliminary transcript, replace only the matching session after verifying its source identity, leaving other sessions intact. Update indexes idempotently so repeated saving does not duplicate rows. Maintain only real pending questions or agreed tasks; label optional practice as suggestions. Create/update the video week's material-collection note at authorized session archiving, recording links, terms, and actual quiz evidence; label it as accumulated material, not a completed weekly review. Create speaking-practice records only if the user actually practiced speaking. A video-only session does not generate speaking statistics, life-event records, or speaking weekly performance claims.

At authorized session archiving, also save the available recording transcript as `对话记录/日期/完整逐字稿.md` and link it from the dialogue record and main index, matching speaking practice. Preserve each source entry exactly, including language, repetitions, recognition errors, speaker labels, and available timing. Exhaust final pagination before calling it complete; label preliminary or unavailable/partial coverage and never reconstruct missing speech. This is the session recording transcript, not a claim to complete original-video subtitles or unrecorded chat messages. Read back saved notes, verify meaningful index links, and report saved locations and material context gaps.

## Weekly review and speaking bridge

Run weekly review when the user asks; do not create reminders or background jobs. Use the same week boundaries, date naming, collapsed answer callouts, and feedback conventions as speaking practice. Follow the shared order:

1. **本周学习感受与视频回顾**: source-linked topics; feelings only if expressed.
2. **本周英语回考**: vocabulary-led questions about meaning, contextual use, new situations, and selected spoken expressions; add a smaller AI concept section when relevant. Prioritize unresolved or hinted items, then sample previously correct items. Change the scenario from closing quizzes instead of merely repeating answers. Keep reference answers collapsed and hidden before the attempt.
3. **本周英语复盘**: actual difficulty/progress evidence, with one-sentence summaries and tables. Unanswered questions remain pending; no claims of retention without a later answer.
4. **本周 To-do check**: unresolved questions and actual agreed practice.
5. **本周总结**: retained English and subject knowledge, within the observed evidence.
6. **下周两个重点**: one language focus and one AI-understanding/application focus (adapt to the video's subject).

Share quiz evidence through links across the two weekly reviews. Test a shared term once in a combined weekly session; separate tests on later dates may provide retention evidence. Do not duplicate questions or copy all answers into both reviews. Keep existing speaking review content intact.

Offer video expressions as optional speaking topics. When the user actually practices, put only their own output and language feedback in the speaking record, link back to the video source, and reuse established error/progress tags. Watching or being shown a model sentence is not evidence of speaking practice. Next-session or weekly reviews read prior records to choose useful items; suggested review times are not automatic follow-up promises.
