# Milestone 1 — Folder Restructure + Planning Files

**Status:** ✅ Complete

## What this milestone does

Sets up the correct folder structure and creates the governance files that all future milestones depend on.

## Tasks

- [x] Create `assets/images/` directory
- [x] Copy all images (my_pic.jpeg, 1st_project.jpg, Portfolio.png, Ai_project.png, Course_1.png, Course_2.png, pic1.jpg) into `assets/images/`
- [x] Update all `src="..."` paths in index.html to `assets/images/...`
- [x] Write `instructions.md` (3 Claude rules)
- [x] Write all 5 milestone .md files

## Folder structure after this milestone

```
Portfolio/
├── index.html
├── instructions.md
├── assets/
│   └── images/
│       ├── my_pic.jpeg
│       ├── 1st_project.jpg
│       ├── Portfolio.png
│       ├── Ai_project.png
│       ├── Course_1.png
│       ├── Course_2.png
│       └── pic1.jpg
└── milestones/
    ├── milestone-1.md
    ├── milestone-2.md
    ├── milestone-3.md
    ├── milestone-4.md
    └── milestone-5.md
```

## Verification

Open `Portfolio/index.html` in browser — all images should still load (profile pic, project cards, cert cards).
