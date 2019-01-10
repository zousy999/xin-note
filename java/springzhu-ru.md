1.静态注入 通过构造器 + 注解  \`@autowired\` Only one constructor can have @Autowired annotation

> ```java
>      @Autowired
>     private AbGroupTagUtils(TaskAbPosMapper taskAbPosMapper) {
>         AbGroupTagUtils.taskAbPosMapper = taskAbPosMapper;
>         init();
>     }
> ```



