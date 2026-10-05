瑶屿 YAOYU 部署包（Netlify Functions + Netlify Blobs）
包含：商品展示首页、商品管理页、持久化商品目录、询盘保存函数。
重要：这是待部署验证的代码包，不是已上线网站。部署前需在 Netlify 站点环境变量设置 ADMIN_PASSWORD（强口令），启用 Netlify Functions/Blobs，并安装依赖后部署。首次部署后用 /admin/ 管理商品。
商品保存在 Netlify Blobs，后续继续使用同一站点和同一 store 即可保留商品。图片以压缩后的 Data URL 存储，建议单张不超过 1.5MB；大规模图片应改用对象存储。
询盘当前保存于 Netlify Blobs，当前版本没有独立询盘管理页面、邮件通知、完整账号系统或权限体系。部署后务必测试商品新增/上下架/删除、前台显示、询盘提交和重新部署后数据是否保留，再正式录入大量产品。
