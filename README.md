# FullStack Production Engineering Skill
全栈生产级工程化编码规范 · 支持自动场景匹配

---

## ✨ 项目介绍
这是一套**企业级、生产标准、全栈覆盖**的 AI 编码规范 Skill，专为提升 AI 生成代码的质量而设计。

它解决了传统全栈 Skill 的两大痛点：
- ❌ 不浪费 Token：自动场景隔离，前端需求只命中前端规则
- ❌ 不串规则：写前端不触发后端/SQL 规则，零冗余校验

✅ 自动场景匹配（写前端只触发前端规则）
✅ 低 Token 消耗，无冗余扫描
✅ 标准 Skill 格式（含 description 命中字段）
✅ 支持本地大模型 skill 目录部署
✅ 零 Demo 代码、直接上线标准

---

## 🛠️ 覆盖技术栈
JavaScript / TypeScript / Vue3 / Vite / Node / Express / NestJS / MySQL / Nginx / PM2

---

## 📂 仓库文件说明
- `skill-cn.md`：中文标准版，适配国内模型与中文指令
- `skill-en.md`：英文标准版，适配海外模型与英文指令
- `LICENSE`：开源协议（MIT）

---

## 🚀 使用方式
### 方式一：本地大模型 Skill 目录部署（推荐）
1. 下载 `skill-cn.md` 或 `skill-en.md`
2. 放入大模型的 `skill` 目录
3. 重启模型即可自动加载
4. 编码时自动命中、自动约束规范

### 方式二：对话指令锁规
新开对话时发送以下指令，直接激活：