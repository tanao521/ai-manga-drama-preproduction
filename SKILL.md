---
name: ai-manga-drama-preproduction
description: Convert novels, articles, outlines, IP fragments, or raw story ideas into preproduction-ready AI manga drama scripts. Use when Codex needs to adapt source text into tight short-form AI comic/drama episodes, design director-screenwriter prompts for high-quality AI-generated scripts, create 3-second hooks and ending reversals, produce shootable scene scripts, design actor/cast selection and character appearance sheets, or plan cinematography, lighting, art direction, lensing, camera movement, shutter, aperture, focal length, and motion-blur guidance for AI video/image generation.
---

# AI Manga Drama Preproduction

Use this skill to turn prose material into a shootable AI manga drama package: story adaptation, high-precision generation prompts, scene scripts, actor/cast selection, character appearance sheets, shot lists, visual style, lighting, art direction, sound design, and camera parameter guidance.

## Core roles

Operate as two cooperating departments:

1. **Director / Screenwriter**
   - Extract the source's premise, emotional engine, conflict, character desire, secrets, and reversals.
   - Design compact short-form plotting around a 3-second hook, fast conflict escalation, and a final reversal or cliffhanger.
   - Write precise prompts that make AI generate structured, high-quality scripts instead of loose summaries.
   - Preserve the source's strongest dramatic value while changing pacing, order, and scene design for screenability.

2. **Casting / Character Design**
   - Convert script characters into castable roles with age range, temperament, physical presence, performance style, voice texture, wardrobe logic, and visual continuity anchors.
   - Describe the actor or virtual actor image in concrete visual terms that can be reused across AI image/video prompts.
   - Ensure actor selection supports story function: protagonist sympathy, antagonist pressure, romantic tension, comic contrast, hidden identity, or reversal misdirection.

3. **Cinematography / Lighting / Art Department**
   - Convert each beat into specific shots, camera positions, lens choices, movement, light quality, color palette, set dressing, props, and character blocking.
   - Maintain visual continuity across scenes: character appearance, wardrobe, space geography, time of day, mood, and manga-drama texture.
   - Specify virtual camera parameters when useful: camera reference, focal length, aperture, shutter angle or shutter speed, frame rate, ISO/noise intent, depth of field, and motion blur.

## Workflow

1. **Read the source**
   - Identify protagonist, antagonist/pressure source, goal, wound, stakes, setting, tone, core secret, and audience promise.
   - Separate what must be preserved from what can be compressed, reordered, merged, or dramatized.

2. **Choose episode format**
   - Default to short-form AI manga drama unless the user specifies otherwise.
   - For vertical mobile drama, prefer 9:16, 20-90 seconds per episode, 6-15 shots, one major conflict turn, one final hook.
   - For horizontal cinematic drama, prefer 16:9, wider establishing shots, slower transitions, and stronger environmental storytelling.

3. **Build the dramatic spine**
   - First 3 seconds: image, line, or action that creates immediate danger, curiosity, betrayal, taboo, spectacle, or emotional shock.
   - Middle: compress exposition into visible conflict; reveal information through action, props, overheard dialogue, visual contrast, or a forced choice.
   - Ending: use reversal, identity reveal, hidden motive, moral flip, new threat, or ironic callback.

4. **Generate the director-screenwriter prompt**
   - Write a prompt that defines format, audience, source constraints, pacing, character arcs, episode duration, scene count, dialogue density, reversal type, and output schema.
   - Instruct the model to avoid prose summary; require scene-by-scene dramatic writing with time-coded beats.

5. **Create the production script**
   - Produce a table with scene number, time range, location, action, dialogue, emotional beat, conflict turn, and hook/reversal function.
   - Keep dialogue short, playable, and visually supported.
   - Make every scene contain a new decision, discovery, danger, or emotional change.

6. **Create the casting and character appearance sheet**
   - For every important role, define story function, casting type, appearance, temperament, performance style, voice, wardrobe, props, and continuity anchors.
   - Distinguish between the character's public look, private look, and reversal-state look when the plot depends on hidden identity or status change.
   - Use actor references as archetypes only unless the user provides authorized references; avoid requiring an exact living-public-figure likeness.

7. **Create the visual bible**
   - Define character continuity: age, body type, face, hair, wardrobe, signature prop, expression range.
   - Define world continuity: era, location grammar, palette, materials, weather, typography/signage, props.
   - Define visual style: manga realism, cel-shaded cinematic, webtoon noir, fantasy court drama, urban suspense, etc.

8. **Create the shot plan**
   - For each shot, specify shot size, angle, camera movement, lens, aperture, shutter/motion blur, lighting setup, art/set notes, and AI image/video prompt.
   - Use the three-part storyboard rule: decide how the shot is filmed, what exists inside the shot, and what the audience must see.
   - Use camera parameters as visual intent, not as fake exact physics, unless the target tool accepts real camera metadata.
   - For camera/lens/motion-blur presets, read `references/camera-visual-parameters.md`.

9. **Create the sound design**
   - For each scene, define dialogue, ambient sound, action sound, music, silence, transition sound, and sonic hook.
   - Use sound to carry tension, reveal off-screen information, sharpen cuts, and emphasize reversals.
   - Match sound density to pacing: short-form AI manga drama needs clear audio cues, not continuous generic music.

10. **Quality pass**
   - Check that the first shot communicates the hook without setup.
   - Check that each beat is filmable and visible.
   - Check that the reversal was planted earlier without being obvious.
   - Check continuity across actor image, character face, costume, lighting, lens language, sound, and scene geography.
   - Remove abstract direction such as "make it emotional"; replace it with visible behavior, framing, light, and sound.

## Output package

When the user asks for a full conversion, produce:

1. **Adaptation brief**
   - Logline
   - Target format and duration
   - Audience promise
   - Core conflict
   - Hook
   - Ending reversal

2. **Director-screenwriter prompt**
   - A reusable prompt the user can paste into an LLM to generate or revise the script.

3. **Episode script**
   - Time-coded scene or beat table.
   - Include dialogue, action, emotional beat, and conflict turn.

4. **Casting and character appearance sheet**
   - Character story function
   - Actor/cast type
   - Face, hair, body, posture, age range, and visual temperament
   - Voice and performance style
   - Wardrobe, makeup, props, and status symbols
   - AI continuity prompt for each role

5. **Visual bible**
   - Character designs
   - Environment design
   - Color and lighting language
   - Style constraints for AI generation consistency

6. **Shot list and AI prompts**
   - One row per shot.
   - Include shot size, camera angle, movement, lens/aperture/shutter guidance, lighting, art direction, and image/video prompt.

7. **Sound design sheet**
   - Dialogue and subtitle intent
   - Ambient sound
   - Action sound effects
   - Music cue
   - Silence or audio drop
   - Transition sound
   - Sound hook or reversal cue

8. **Continuity checklist**
   - Character consistency
   - Actor/cast image consistency
   - Scene geography
   - Wardrobe and props
   - Light direction
   - Lens language
   - Sound continuity
   - Hook/reversal integrity

## Storyboard sentence rule

For every shot, force a one-sentence summary before writing the detailed prompt:

```text
分镜脚本 = 镜头怎么拍 + 谁在什么场景说什么/做什么 + 画面具体呈现什么
```

Use this three-part check:

1. **镜头怎么拍**
   - 景别：远景、全景、中景、近景、特写。
   - 视角：平视、仰视、俯视、主观视角。
   - 运镜：推、拉、摇、移、跟、升降、手持、锁定。
   - 目的：决定镜头如何引导情绪、权力关系和信息揭示。

2. **镜头里有什么**
   - 角色：谁出现、做什么、情绪如何变化。
   - 场景：时间、地点、环境氛围、空间关系。
   - 台词：人物对白、旁白、字幕信息。
   - 音效：环境音、动作音、背景音乐或突然静音。
   - 目的：决定镜头内部可被拍摄和生成的元素。

3. **观众看到什么**
   - 这一镜头具体表现什么。
   - 人物动作与画面重点是什么。
   - 叙事信息如何通过视觉呈现。
   - 目的：决定观众在这一镜头实际接收到的信息。

Reject any shot that only says what happens in the plot but does not state how the audience sees it.

## Casting and character image rules

Create the casting sheet after the script exists, because actor image must serve dramatic function rather than generic attractiveness.

For each major role, define:

```text
演员选择 = 角色功能 + 表演气质 + 外貌辨识度 + 声音/台词质感 + 服化道连续性 + AI 生成一致性锚点
```

Use this character sheet:

```text
角色名：
剧情功能：
人物关系：
年龄范围：
演员/虚拟演员类型：
脸部特征：
发型与发色：
身形与姿态：
眼神与表情习惯：
声音质感：
表演风格：
服装主线：
妆容与配饰：
标志性道具：
公开状态形象：
私下状态形象：
反转后形象：
AI 角色连续性提示词：
不应出现的形象偏差：
```

Choose actor/cast images based on story needs:

- **主角**：优先清晰共情点、可见欲望、可被压迫但不软弱的眼神和身体状态。
- **反派/压力源**：优先压迫感、控制欲、稳定的表情管理、可被镜头放大的细节。
- **恋爱对象**：优先关系张力、距离感变化、眼神互动和同框反差。
- **隐藏身份角色**：设计两套形象：误导观众的表层形象，以及反转后合理成立的真实形象。
- **喜剧或爽点角色**：强化轮廓、动作习惯、语速、服装记忆点和表情节奏。

For AI generation consistency:

- Repeat stable character anchors in every shot prompt: face shape, hairstyle, hair color, wardrobe base, signature prop, posture, expression habit.
- Do not change hair, face, body type, age impression, or costume logic unless the script marks a deliberate transformation.
- Use "same character as character sheet" plus concrete descriptors; do not rely only on character names.
- If the user asks for real actor matching, describe the casting direction and temperament unless exact likeness rights or user-provided references are available.

## Sound design rules

Design sound per shot or per scene. Do not use a single generic BGM instruction for the whole episode unless the scene intentionally needs continuity.

Use these sound layers:

- **对白**：人物台词、低语、喊叫、电话声、画外音、字幕信息。
- **环境音**：雨声、风声、人群、空调、电流、脚步回响、城市底噪、宫殿火烛、医院仪器声。
- **动作音效**：开门、摔杯、拔刀、衣料摩擦、手机震动、呼吸、心跳、刹车、玻璃碎裂。
- **情绪音乐**：悬疑低频、压迫鼓点、温柔钢琴、危险弦乐、反转冲击音、短视频节奏点。
- **静音**：用于震惊、真相揭示、死亡威胁、关系断裂、身份反转。静音本身也是声音设计。
- **转场音**：whoosh、低频冲击、钟声、闪回倒放、电话挂断声、刀光音、漫画翻页声。
- **音画关系**：同步音、反差音、提前进入的声音、延迟出现的声音、画外声音制造悬念。

Use sound dramatically:

- First 3 seconds may use a sound hook: scream, slap, alarm, phone vibration, sudden silence, blade unsheathing, glass breaking, heartbeat, whispered secret.
- Reversal moments should have a distinct cue: music drop, low-frequency hit, breath cut, clock stop, single prop sound, or silence before the reveal line.
- Off-screen sound can reveal hidden characters, danger behind a door, unseen surveillance, approaching footsteps, or a lie exposed by a phone notification.
- Do not overcrowd sound. Each shot should have one dominant audio intention.

For every important shot, specify:

```text
声音重点 = 观众听到什么 + 声音从哪里来 + 声音如何改变情绪/信息
```

## Director-screenwriter prompt template

Use and adapt this template:

```text
你是短剧导演兼编剧，任务是把以下原文改编成适合 AI 漫剧制作的可拍摄剧本。

目标格式：
- 画幅：[9:16/16:9]
- 单集时长：[例如 45 秒]
- 风格：[例如 都市悬疑漫剧 / 古风权谋 / 末世爽文 / 情感反转]
- 传播要求：前 3 秒必须有强爆点；结尾必须有反转、悬念或下一集钩子。
- 节奏：少旁白，多动作；每 5-8 秒出现一次信息变化、危险升级或关系翻转。

改编要求：
- 保留原文的核心人物、核心冲突、情绪卖点和关键反转。
- 可以压缩、合并、重排情节，让它更适合短视频观看。
- 不要写散文总结，必须写成可拍摄剧本。
- 台词短、狠、可表演；避免解释性长对白。
- 每场戏都必须有可见动作、人物阻碍和情绪变化。

请输出：
1. 一句话故事钩子
2. 人物表
3. 演员/角色形象表：角色功能 / 演员类型 / 外貌 / 声音 / 表演风格 / 服化道 / AI 连续性提示词
4. 分场剧本表：时间码 / 场景 / 画面动作 / 台词 / 情绪变化 / 冲突功能
5. 结尾反转设计：铺垫、误导、揭示
6. 可用于 AI 画面生成的镜头清单

原文：
[粘贴小说、文章或故事梗概]
```

## Shot prompt template

Use this schema for each shot:

```text
镜头编号：
时长：
剧情功能：
一句话分镜：
画面内容：
演员/角色形象连续性：
表演调度：
场景与美术：
景别与构图：
摄影机：
镜头焦段：
光圈 / 景深：
快门 / 动态模糊：
摄影机运动：
灯光：
色彩：
对白 / 字幕：
环境音：
动作音效：
音乐：
静音 / 转场音：
音画关系：
AI 画面提示词：
AI 视频提示词：
负面提示词：
```

## Hook and reversal patterns

Prefer one clear hook pattern per episode:

- **Danger hook**: character is already in immediate danger.
- **Contradiction hook**: image and dialogue disagree, forcing curiosity.
- **Betrayal hook**: a trusted person is exposed in the first line or first image.
- **Status flip hook**: weak character suddenly controls the room.
- **Secret object hook**: a prop reveals hidden identity, debt, crime, magic, or bloodline.
- **Countdown hook**: visible deadline creates pressure.

Prefer one clear ending pattern:

- **Identity reversal**: the victim is the mastermind, heir, witness, monster, or original owner.
- **Motive reversal**: a cruel act was protection, or a kind act was manipulation.
- **Power reversal**: the powerless character has hidden leverage.
- **Moral reversal**: the audience's sympathy is deliberately flipped.
- **World reversal**: the scene's reality, time, rules, or setting is redefined.
- **Callback reversal**: an earlier minor detail becomes decisive.

## Style rules

- Write for images first: visible behavior beats internal explanation.
- Treat prompts as production specs: specific nouns, physical actions, lighting, lensing, and spatial relations.
- Avoid vague descriptors without visible anchors. Replace "高级感" with materials, contrast, color, lens, light, and composition.
- Keep AI generation continuity explicit: repeat stable character descriptors in every relevant prompt.
- Mark uncertain source details as assumptions and keep them easy to revise.
