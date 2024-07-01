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
- uses: Platane/snk@v3
  with:
    # github user name to read the contribution graph from (**required**)
    # using action context var `github.repository_owner` or specified user
    github_user_name: ${{ github.repository_owner }}

    # list of files to generate.
    # one file per line. Each output can be customized with options as query string.
    #
    #  supported options:
    #  - palette:     A preset of color, one of [github, github-dark, github-light]
    #  - color_snake: Color of the snake
    #  - color_dots:  Coma separated list of dots color.
    #                 The first one is 0 contribution, then it goes from the low contribution to the highest.
    #                 Exactly 5 colors are expected.
    outputs: |
      dist/github-snake.svg
      dist/github-snake-dark.svg?palette=github-dark
      dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
