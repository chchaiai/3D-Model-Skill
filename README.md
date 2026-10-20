# 3D Model Skill

可复用的 Codex 3D 建模技能。覆盖资料与几何、构造细节、PBR 材质、光照反射、LOD、加载、交互及验证交付。

适用于建筑、校园、园区和一般物体的新建或优化，按任务选择工作步骤，沿用现有技术栈。

## 安装

将本仓库复制到 Codex 技能目录下的 `3d-model-skill` 文件夹，保证结构为：

```text
~/.codex/skills/3d-model-skill/
├── SKILL.md
└── agents/openai.yaml
```

也可执行：

```sh
git clone https://github.com/chchaiai/3D-Model-Skill.git ~/.codex/skills/3d-model-skill
```

安装后新开 Codex 对话。如果技能未出现，重启 Codex 后再检查。

## 使用

```text
使用 $3d-model-skill，根据这些照片和尺寸建立模型，输出可编辑源文件与GLB。
```

```text
使用 $3d-model-skill 优化当前校园模型的玻璃、墙面和屋顶，保留建筑布局，验证手机交互与首次加载。
```

默认允许按任务自动选择，也可通过 `$3d-model-skill` 显式调用。

## 原则

- 资料保留来源，区分已确认、估算与未知。
- 先空间与构造，再材质与光照。
- 保留优化范围，使用可比较、可回退的改动。
- 性能和质量用目标环境中的证据说明。
- 交付可编辑、可运行、可恢复的实际成果。

完整执行说明见 [SKILL.md](SKILL.md)。本技能不附带模型、照片或第三方材质，资源许可由具体项目核对。
