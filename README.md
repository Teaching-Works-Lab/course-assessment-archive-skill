# Course Assessment Archive Skill

面向沧州交通学院课程考核与试卷资料归档的 Codex Skill。它依据现行制度，从任课教师、课程负责人、教学秘书/专业和学院四个默认角色位置，回答材料应该放在哪一层、缺少什么、由谁整改以及如何复核。

显式触发名称：`$course-assessment-archive`

## 主要用途

- 生成可复制的课程考核资料目标目录树；
- 将已有文件映射到完整相对归档路径；
- 区分正考/补考、考试课/考查课及试卷/非试卷考核分支；
- 按角色检查课程、教师、教学班和学院范围的覆盖情况；
- 识别常见归档错误，并把整改任务交还实际责任人；
- 在取得新版制度文件或经核实的纠错后，受控更新规则。

它不负责试卷 Word 格式对比、套模板或题目内容校验；这些任务由 [`exam-word-skill`](https://github.com/Teaching-Works-Lab/exam-word-skill) 处理。

## 使用示例

```text
$course-assessment-archive 我是任课教师，请按现行规范告诉我这门课每个文件应该放到哪里。
```

```text
$course-assessment-archive 我是教学秘书，请检查本专业课程、教师和教学班的归档覆盖情况。
```

## 安装

```powershell
git clone https://github.com/Teaching-Works-Lab/course-assessment-archive-skill.git "$env:USERPROFILE\.codex\skills\course-assessment-archive"
```

重新启动 Codex 后即可使用。
