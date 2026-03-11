# 三年终止协议执行指南 (Termination Protocol Guide)

> "最好的陪伴，是当你已经足够强大去面对生活，而我已悄然隐入岁月。"

## 1. 触发机制 (The Trigger)
当系统时钟（local_system_clock）检测到当前时间 >= `protocol_meta.created_at + 1095 days` 时，系统自动进入“不可逆安全删除逻辑”。
* **无干扰原则：** 系统运行期间（1-1095天），严禁以任何 UI 形式显示倒计时、提醒或生存进度条，确保生者不受“截止日期”的心理压迫。

## 2. 不可逆安全删除逻辑 (Irreversible secure deletion Logic)
倒计时归零后，后端脚本必须执行以下操作以符合 **AGPL-3.0** 下的隐私承诺：
* **模型碎纸机：** 调用 `delete_directory_recursive()` 或同等指令，粉碎 `./models/` 下的所有权重文件。
* **向量抹除：** 清空 FAISS/ChromaDB 等本地向量数据库。
* **日志清理：** 擦除所有交互产生的临时文件（Cache）与日志（Logs）。
* **进程终止：** 脚本执行 `terminate_service_process()`，并自删除启动项。

## 3. 留存说明 (What Remains)
根据协议，系统销毁的是“AI 人格层”，而用户生前录入的原始素材（Raw Media）应由生者自行保管，作为普通家庭档案永久留存。
