# AGENTS.md - Guide for Home Construction Planning Repository

This is a **documentation and research knowledge base** for home construction in Thailand - not a traditional code repository.

## Repository Structure

```
home_making_plan/
├── assets/                  # Reference documents and images
│   ├── block-images/       # Material reference images
│   └── *.md                # Quick reference guides
├── research/               # In-depth research reports
│   └── *-YYYY-MM-DD.md    # Dated research documents
└── *.skill                 # Binary skill definition files
```

## File Naming Conventions

Research files: `{topic}-{slug}-{YYYY-MM-DD}.md` (e.g., `brick-types-research-thai-construction-2026-01-18.md`)
Asset files: `{topic}-{type}.md` for guides, `{material-type}-{number}.{ext}` for images

## Document Standards

### Header Metadata (Research Files)
```markdown
# Title (Thai/English bilingual)
**วันที่:** DD MMMM YYYY
**ระดับ:** Standard Research | Deep Research
**สถานะ:** สมบูรณ์ | ร่าง
**Research Method:** [Tool used] with [expertise domain]
**Language:** Bilingual (Thai/English) | Thai | English
---
## Executive Summary (สรุปภาพรวม)
[Brief overview]
**Claim 1:** [Statement] - **Confidence:** HIGH/MEDIUM/LOW - **Reason:** [Justification] - **Sources:** [1][2]
---
```

### Table of Contents
Include anchor-linked TOC after Executive Summary:
```markdown
## Table of Contents
1. [Section One](#section-one)
2. [Sources](#sources)
---
```

## Content Style Guidelines

### Bilingual Content
- Primary: Thai (local context), Secondary: English (technical terms)
- Format: `## Thai Title (English Title)` or `คำศัพท์ไทย (English Term)`

### Tables
Use pipe tables with alignment and bilingual headers:
```markdown
| ประเภท | Type | คำอธิบาย | Description |
|---|---|---|---|
```

### Standards References
- Format: `มอก. 77 (TIS 77) - [Description]`
- Always add: `*ตรวจสอบฉบับล่าสุด*` / `*Verify current revision*`

### Source Citations
Numbered brackets `[1]` in-text, with Sources section at end:
```markdown
## Sources
[1] Source Title - URL or publication info
```

## Diagram Formatting
Use code blocks for text-based diagrams:
```markdown
```
┌─────────────────────────────────────┐
│           Layer 1                    │
└─────────────────────────────────────┘
```
```

## Image Management
- Store in `assets/block-images/`
- Names: `{material-type}-{number}.{ext}` (lowercase, hyphens)
- Include alt text: `
![Description](../assets/block-images/filename.jpg)
`

## Claims and Confidence Levels
- **HIGH:** Multiple authoritative sources, industry standard
- **MEDIUM:** Several sources agree with some variance, expert consensus
- **LOW:** Limited sources, conflicting information, requires verification
Always include reasoning and source citations.

## Thai Language Conventions
Common terms: อิฐมอญ (Clay brick), บล็อกคอนกรีต (Concrete block), อิฐมวลเบา (AAC block), เสาเข็ม (Pile), คาน (Beam), พื้น (Slab)
Dates: `3 กุมภาพันธ์ 2026` or `2026-02-03`

## When Creating/Editing Documents
1. Check existing patterns - look at similar research files first
2. Maintain bilingual format - Thai primary, English secondary
3. Include metadata header - Date, level, status, method
4. Add citations - Reference sources with numbered brackets
5. Use consistent terminology - Match Thai/English terms used elsewhere
6. Test TOC links - Ensure anchor links work after saving

## No Build/Test Commands
This repository contains only documentation. Agents focus on:
- Document organization and structure
- Content accuracy and sourcing
- Markdown formatting consistency
- Bilingual terminology alignment
- Image asset management

## Key Topics Covered
Brick/block materials, foundation systems, soil settlement, construction costs, room-by-room recommendations, TIS/มอก. standards, Thai climate (hot-humid)
