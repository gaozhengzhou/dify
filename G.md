## 去掉sysQueryInUser校验
web/app/components/workflow/nodes/llm/default.ts
```
// if (!errorMessages && !!payload.memory) {
//   const isChatModel = payload.model.mode === 'chat'
//   // payload.memory.query_prompt_template not pass is default: {{#sys.query#}}
//   if (isChatModel && !!payload.memory.query_prompt_template && !payload.memory.query_prompt_template.includes('{{#sys.query#}}'))
//     errorMessages = t('workflow.nodes.llm.sysQueryInUser')
// }
```

web/app/components/workflow/nodes/llm/panel.tsx
```
{/*{inputs.memory.query_prompt_template && !inputs.memory.query_prompt_template.includes('{{#sys.query#}}') && (*/}
{/*  <div className='leading-[18px] text-xs font-normal text-[#DC6803]'>{t(`${i18nPrefix}.sysQueryInUser`)}</div>*/}
{/*)}*/}
```