## Hi there 👋

<!--
**Bio-WYX/Bio-WYX** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
-->
- 🔭 生信工程师
- 🌱 python、R、perl
  - NGS数据分析、流程开发
  - python数据库爬取、数据统计
  - 机器学习
- 📫 imauwyxbio@gmail.com

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=Bio-WYX&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)

name: Waka Readme

on:
  # for manual workflow trigger
  workflow_dispatch:
  schedule:
    # runs at 12 AM UTC (5:30 AM IST)
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: WakaReadme DevMetrics
    runs-on: ubuntu-latest
    steps:
        # this action name
      - uses: athul/waka-readme@master # do NOT replace with anything else
        with:
          GH_TOKEN: ${{ secrets.GH_TOKEN }} # optional if on profile readme
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }} # required
          ### meta
          API_BASE_URL: https://wakatime.com/api # optional
          REPOSITORY: YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME # optional
          ### content
          SHOW_TITLE: true # optional
          SECTION_NAME: waka # optional
          BLOCKS: -> # optional
          CODE_LANG: rust # optional
          TIME_RANGE: all_time # optional
          LANG_COUNT: 10 # optional
          SHOW_TIME: true # optional
          SHOW_TOTAL: true # optional
          SHOW_MASKED_TIME: false # optional
          STOP_AT_OTHER: true # optional
          IGNORED_LANGUAGES: YAML JSON TOML # optional
          ### commit
          COMMIT_MESSAGE: Updated waka-readme graph with new metrics # optional
          TARGET_BRANCH: master # optional
          TARGET_PATH: README.md # optional
          COMMITTER_NAME: GitHubActionBot # optional
          COMMITTER_EMAIL: action-bot@github.com # optional
          AUTHOR_NAME: YOUR_NAME # optional
          AUTHOR_EMAIL: YOUR@EMAIL.com # optional
          # you can populate email-id with secrets instead
