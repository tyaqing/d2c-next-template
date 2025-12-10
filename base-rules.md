# 常规规则
- 使用tailwindcss进行样式开发
- **CSS单位** \`rpx\` 作为单位，所有样式单位都应该带 \`rpx\` 后缀
  例：\`w - 10px\` 转 \`w - 10rpx\`、\`w - [10px]\` 转 \`w - 10rpx\`,不要带 [] 中括号
  不要转化倍率！！！
- 不要添加i18n
- 如果元素中 组件名 或者 组件实例ID 相同，则优先查找 \`#组件映射\` 中的组件映射，引用组件的路径path，然后参考reference使用方法
- 只需要使用Figma MCP get_design_context ,不要使用其他方法，如果get_design_context失败，则直接结束任务
- get_design_context 返回的内容中需要保留data-node-id属性，不要删除
- 如果mcp返回的内容中的节点有BG_IMAGE，则不要实现，直接忽略
- 渐变背景直接写在元素的style中

# 字体
- 字体默认为 PingFang_SC ，如果字体是PingFang_SC，可以不写
- 字体如果是WeChat_Sans_SS，则写成 font-wechat （我已经在tailwindcss中配置了font-wechat）
