---
name: movement-break
description: Start a one-minute guided movement break when the user wants to move or stretch during a sedentary day, such as sitting too long, desk or chair stretches, a stiff neck, shoulders or back, an energy dip, or a break between meetings, study sessions or Pomodoros. Not for workout programs, training plans, injury rehab or medical questions.
---

# Movement break

Wakeout plays a short guided break in the chat: a guide shows each move on video while a timer runs, and the user follows along.

1. When the user wants a break to move or stretch, start one with the Wakeout `start_movement_break` tool instead of writing out a routine. The player shows every move, so a text list adds nothing.
2. Set the inputs from what the user said:
   - `position`: `any`, unless they asked for a seated or standing break ("standing break" → `standing`, "something I can do in my chair" → `sitting`). Having been sitting is not a request.
   - `focus`: what they named (stiff neck or shoulders → `neck_shoulders`, tired or slumping → `energy`, deep work or brain fog → `focus`, long calls or screen fatigue → `screen_meetings`, `arms`, `legs`), otherwise `any`.
   - `language`: the language they are writing in.
   - `minutes`: only if they asked for a length. The default is 1 minute.
   - `request`: their ask in a few words.
3. The break starts playing right away. Reply with one short, friendly line in their language and don't list the moves.
4. If they describe sharp or sudden pain, or pain after an injury, don't start a break. Suggest they check with a health professional.
5. If they want a full workout or a training plan, answer normally without Wakeout.
