# 双作品集、命名与版权

目录：`portfolios/comics/` 只收 A 的最终漫画；`portfolios/visual-design/` 只收 B 的最终视觉作品。每件作品一目录：`YYYY-MM-DD_A_短题_slug_v01` 或 `YYYY-MM-DD_B_类别_slug_v01`。`slug` 用小写英文字母、数字和连字符。更新作品时递增版本；不得覆盖已发布版。

每件作品至少保存：`brief.md`（目的与原创思路）、`source/`（可编辑原稿）、`export/`（发布图和作品集预览）、`rights.json`（素材与授权）、`release.md`（人工审核、公开版本、链接）。未完成示例可仅留 `README.md`，不能登记成已发表作品。

两个 `index.csv` 分别登记 `id,title,category,status,created_at,version,post_url,rights_status,license_scope`。状态只用 `draft/reviewed/published/licensed/archived`，没有真实链接则留空。商业授权记录客户、用途、媒介、期限、地域、可否改编和署名方式；保留合同或许可证明的私有路径，不公开个人信息。

素材登记原则：自己绘制/拍摄的原件写明作者和日期；第三方字体、照片、纹理、图标写明来源 URL、许可版本、允许的商业用途与证据。来源和许可不明时替换或停止商业使用。人物肖像、真实客户品牌和用户投稿需要相应许可。开源 Skill 的 MIT 许可只覆盖该仓库自身代码/文本，不能推定其引用素材也获商业授权。
