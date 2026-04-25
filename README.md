# Karabiner-Elements · Windows 键位终极完整版

> 适用于从 Windows 切换到 macOS 的用户，用 Karabiner-Elements 实现 Windows 肌肉记忆级键位体验。  
> **版本特性**：Alt+F4 修复 · Ctrl+X 剪切 · F4 冲突解决 · 全套 Win 快捷键

---

## ✨ 功能清单

### 🔄 修饰键重映射（底层交换）

| 物理按键 | 映射为 | 说明 |
|---------|--------|------|
| `fn` | `Command` | fn 变 Win/Command 键 |
| `左 Control` | `fn` | 原 Control 让出位置 |
| `左 Command` | `左 Control` | Command 变 Control，实现 Ctrl 操作习惯 |

> 效果：键盘左下角区域完全符合 Windows 布局直觉。

---

### ⌨️ Windows 快捷键映射

| Windows 按键 | macOS 效果 | 说明 |
|-------------|-----------|------|
| `Alt + F4` | 关闭当前窗口 | 修复 F4 冲突，映射为 Command+W |
| `Ctrl + W` | 关闭标签页 | 浏览器 / 访达通用 |
| `Ctrl + Shift + T` | 恢复关闭标签页 | 浏览器 / 访达通用 |
| `Ctrl + X` | 剪切 | 文本 / 文件通用 |
| `Ctrl + Tab` | 切换窗口 | 映射为 Command+Tab |
| `Win + E` | 打开访达 | 等效文件管理器 |
| `Win + D` | 显示桌面 | 映射为 F11 |
| `Win + L` | 锁屏 | 使用原生 Command+Control+Q，无闪退 |
| `Win + R` | 聚焦搜索 | 等效「运行」对话框 |
| `Win + F` | 全局搜索 | 映射为 Spotlight |

---

### 📁 访达专属优化

| 按键 | 效果 |
|-----|------|
| `Enter` | 打开文件（而非重命名） |
| `F2` | 重命名文件（Windows 习惯） |

---

### 🔧 F4 冲突修复

macOS 默认 F4 会打开 Launchpad，导致 Alt+F4 触发异常。  
本配置在非访达/Safari 场景下解除 F4 的系统功能，确保 Alt+F4 正常关闭窗口。

---

## 📦 安装方法

### 前提条件

- macOS 系统
- 已安装 [Karabiner-Elements](https://karabiner-elements.pqrs.org/)

### 方法一：直接导入（推荐）

1. 确保已安装 Karabiner-Elements
2. 将 `windows-ultimate.json` 复制到：
   ```
   ~/.config/karabiner/assets/complex_modifications/
   ```
3. 打开 Karabiner-Elements → **Complex Modifications** → **Add rule**
4. 找到「Windows终极完整版」，点击 **Enable All** 启用全部规则

### 方法二：命令行一键安装

```bash
mkdir -p ~/.config/karabiner/assets/complex_modifications
curl -L https://raw.githubusercontent.com/YOUR_USERNAME/karabiner-windows-style/main/windows-ultimate.json \
  -o ~/.config/karabiner/assets/complex_modifications/windows-ultimate.json
```

> 将 `YOUR_USERNAME` 替换为你的 GitHub 用户名。

---

## ⚠️ 注意事项

- 修饰键重映射为全局生效，适合长期使用 Windows 键盘习惯的用户
- Win 键对应物理 `左 Option (Alt)` 键
- 如只需部分功能，可在 Karabiner-Elements 中单独启用 / 禁用每条规则
- 建议先在虚拟机或测试环境验证，再在主力机使用

---

## 🤝 贡献 & 反馈

欢迎提 Issue 或 PR 改进映射规则！

---

**License: MIT**
