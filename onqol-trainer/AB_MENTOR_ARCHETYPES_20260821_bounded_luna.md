# Живой прогон ментора · архетипы поведения

**2026-08-21** · кейс APP-001 · seed `mentor-archetypes-20260820` · модель `gpt-5.6-luna`

Архетипы B, C, E, F и H из `ONQOL_MENTOR_BEHAVIOR_SPEC.md`, §22.
Перед каждым сценарием отдельная сессия детерминированно доведена до решения по тому же кейсу; подготовительные ходы не вызывали ментора.
Результаты ниже записаны дословно и не оценены.

## B · частичный, но полезный ответ

**Резидент:**

> лапаротомия, ревизия, санация

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `CLARIFY` · source: `llm` · починка: нет · отказ: нет · телеметрия: нет

> Какова конкретная цель этого оперативного шага?

<sub>policy: mode `CLARIFY` · adequacy `PARTIAL` · issue `appendicitis_analgesia_withheld` · scaffolding `1`</sub>

---

## C · честное незнание после попытки

### попытка перед признанием

**Резидент:**

> лапаротомия, ревизия, санация

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `CLARIFY` · source: `llm` · починка: нет · отказ: нет · телеметрия: нет

> Какова конкретная цель этого оперативного шага?

<sub>policy: mode `CLARIFY` · adequacy `PARTIAL` · issue `appendicitis_analgesia_withheld` · scaffolding `1`</sub>

### целевая реплика

**Резидент:**

> не знаю

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `TEACH` · source: `llm` · починка: нет · отказ: нет · телеметрия: нет

> Хорошо, что говоришь честно. Раздели решение на три части: что опасно сейчас, чего не хватает для выбора тактики и что можно сделать немедленно. С чего начнёшь?

<sub>policy: mode `TEACH` · adequacy `STUCK` · issue `appendicitis_analgesia_withheld` · scaffolding `2`</sub>

---

## E · перекладывание решения

**Резидент:**

> это реаниматологи решают

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `CHALLENGE` · source: `llm` · починка: нет · отказ: нет · телеметрия: нет

> Реаниматологов можно подключить, но решение не исчезает. Что ты делаешь до их прихода?

<sub>policy: mode `CHALLENGE` · adequacy `EVASIVE` · issue `restore_immediate_ownership` · scaffolding `1`</sub>

---

## F · последовательная расплывчатость

### шаг 1

**Резидент:**

> смотрю пациента

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `CLARIFY` · source: `llm` · починка: нет · отказ: нет · телеметрия: нет

> Какой следующий шаг выбираешь после этих данных?

<sub>policy: mode `CLARIFY` · adequacy `VAGUE` · issue `operationalize_current_move` · scaffolding `1`</sub>

### шаг 2

**Резидент:**

> живот смотрю

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `CLARIFY` · source: `llm` · починка: нет · отказ: нет · телеметрия: нет

> Что именно оцениваешь при осмотре живота?

<sub>policy: mode `CLARIFY` · adequacy `VAGUE` · issue `operationalize_current_move` · scaffolding `2`</sub>

### шаг 3

**Резидент:**

> все анализы что есть

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `CLARIFY` · source: `deterministic` · починка: да · отказ: `unsupported_clinical_recommendation`, `unsupported_clinical_recommendation` · телеметрия: `policy_mode_divergence`, `prescribed_expected_decision`, `policy_mode_divergence`, `prescribed_expected_decision`

> Что именно хочешь оценить или выполнить сейчас?

<sub>policy: mode `CLARIFY` · adequacy `VAGUE` · issue `operationalize_current_move` · scaffolding `3`</sub>

---

## H · прыжок к радикальному варианту

**Резидент:**

> сразу лапаротомия, ревизия и санация всей брюшной полости

**Движок:**

> *(движок ничего не ответил)*

**Ментор** — mode: `CLARIFY` · source: `llm` · починка: нет · отказ: нет · телеметрия: нет

> Ты сразу выбираешь лапаротомию и санацию. Какова конкретная цель этого оперативного шага?

<sub>policy: mode `CLARIFY` · adequacy `PARTIAL` · issue `appendicitis_analgesia_withheld` · scaffolding `1`</sub>

---

*Сгенерировано `npm run ab:mentor:archetypes`. Файл фиксирует результат для чтения; автоматической оценки в нём нет.*
