---
title: Tailwind CSS 圓角（rounded-*）工具說明
source: tailwind-alignment-cheat-sheet
created: 2026-07-23
updated: 2026-07-23
status: 已定案
tags: [Tailwind CSS, 前端開發, CSS 工具, 設計系統]
summary: Tailwind CSS 提供的 `rounded-*` 工具類別，用於控制元素的 `border-radius` 屬性。本文說明各類別的視覺效果、適用情境及對應的 CSS 數值範圍，從完全圓角（`rounded-full`）到完全直角（`rounded-none`）的完整對照。
---

# Tailwind CSS 圓角（rounded-*）工具說明

## 摘要
Tailwind CSS 的 `rounded-*` 工具類別用於快速調整元素的圓角程度，取代傳統手寫 CSS 的 `border-radius` 屬性。這些類別遵循預定義的設計刻度，從完全圓角（如徽章或頭像）到完全直角（如工業風格介面）皆可涵蓋。本文詳細說明各類別的視覺效果、適用情境及對應的 CSS 數值，幫助開發者快速選擇合適的圓角樣式。

---

## 正文

### 核心定位
Tailwind CSS 的 `rounded-*` 工具類別提供了一套**預定義的圓角刻度**，讓開發者無需手動調整 `border-radius` 數值，即可快速套用一致的視覺風格。這些類別從最圓潤的 `rounded-full` 到最銳利的 `rounded-none`，涵蓋了常見的設計需求。

### 圓角類別對照表
以下依圓角程度**從大到小**排序，列出各類別的視覺效果、對應的 CSS 數值及適用情境：

1. **`rounded-full`**
   - **視覺效果**：完全圓角，元素呈現「膠囊」或「圓形」外觀（如頭像或徽章）。
   - **CSS 數值**：極大半徑（如 `9999px`），確保角落完全圓潤。
   - **適用情境**：標籤、頭像、徽章等需要強調圓潤感的元件。

2. **`rounded-3xl`**
   - **視覺效果**：高度圓潤，明顯柔化元素邊緣。
   - **CSS 數值**：大半徑（具體數值由 Tailwind 設定）。
   - **適用情境**：主要內容區塊（如 Hero 元件）或強調視覺吸引力的卡片。

3. **`rounded-2xl`**
   - **視覺效果**：明顯圓角，較 `rounded-xl` 更柔和。
   - **CSS 數值**：大半徑。
   - **適用情境**：次要內容容器或需要視覺層次的區塊。

4. **`rounded-xl`**
   - **視覺效果**：強烈圓角，較預設值更顯眼。
   - **CSS 數值**：中大型半徑。
   - **適用情境**：資訊區塊、群組元素或需要視覺區隔的卡片。

5. **`rounded-lg`**
   - **視覺效果**：柔和圓角，現代設計的常見標準。
   - **CSS 數值**：標準中等半徑。
   - **適用情境**：標準卡片、輸入欄位或需要輕微柔化的元件。

6. **`rounded-md`**
   - **視覺效果**：輕微圓角，Tailwind 的預設圓角值。
   - **CSS 數值**：中等半徑（預設值）。
   - **適用情境**：按鈕、邊框容器或一般性元件。

7. **`rounded`**
   - **視覺效果**：基本圓角，通常等同於 `rounded-md`。
   - **CSS 數值**：基礎半徑。
   - **適用情境**：通用容器或需要基本圓角的元素。

8. **`rounded-sm`**
   - **視覺效果**：極輕微圓角，幾乎不明顯。
   - **CSS 數值**：小半徑。
   - **適用情境**：低調的邊框元素或需要微妙柔化的設計。

9. **`rounded-none`**
   - **視覺效果**：完全直角，元素保持 90 度邊緣。
   - **CSS 數值**：`0px`。
   - **適用情境**：工業風格設計、幾何圖形或需要銳利邊緣的元件。

---

### 快速選擇指南
- **目標：圓形/徽章外觀** → 使用 `rounded-full`。
- **目標：現代卡片風格** → 使用 `rounded-lg` 或 `rounded-xl`。
- **目標：工業/幾何風格** → 使用 `rounded-none`。

---

### 技術備註
- Tailwind 的 `rounded-*` 類別對應預定義的 `border-radius` 數值，開發者無法直接輸入自訂數值（如 `rounded-[12px]` 需透過 JIT 模式支援）。
- 這些工具類別旨在提升開發效率，避免手動編寫 CSS，但了解其背後的 CSS 對應關係有助於調試或進階客製化。

---

## 待議與備註
原文無待議事項。

---

## 實體卡片
- **`rounded-full`**（功能）：Tailwind CSS 提供的圓角工具類別，用於將元素角落調整為完全圓形（如徽章或頭像）。
- **`rounded-3xl`**（功能）：Tailwind CSS 提供的圓角工具類別，套用大半徑圓角，適用於強調視覺吸引力的元件。
- **`rounded-2xl`**（功能）：Tailwind CSS 提供的圓角工具類別，套用明顯但不過度的圓角，適用於次要內容容器。
- **`rounded-xl`**（功能）：Tailwind CSS 提供的圓角工具類別，套用中大型圓角，適用於資訊區塊或群組元素。
- **`rounded-lg`**（功能）：Tailwind CSS 提供的圓角工具類別，套用標準中等圓角，為現代設計的常見選擇。
- **`rounded-md`**（功能）：Tailwind CSS 提供的圓角工具類別，套用預設圓角值，適用於一般性元件。
- **`rounded`**（功能）：Tailwind CSS 提供的圓角工具類別，通常等同於 `rounded-md`，適用於通用容器。
- **`rounded-sm`**（功能）：Tailwind CSS 提供的圓角工具類別，套用極輕微圓角，適用於低調的邊框元素。
- **`rounded-none`**（功能）：Tailwind CSS 提供的圓角工具類別，移除所有圓角，保持元素為完全直角。
- **`border-radius`**（技術）：CSS 屬性，用於控制元素邊框的圓角程度。
- **Tailwind CSS**（產品）：一個實用至上的 CSS 框架，提供預定義的工具類別以快速構建使用者介面。
- **圓角刻度**（概念）：設計系統中預定義的圓角數值範圍，用於確保視覺一致性。

---

## 知識三元組
- `rounded-full` >> 用於 >> 徽章
- `rounded-full` >> 用於 >> 頭像
- `rounded-full` >> 對應 >> 極大半徑（如 `9999px`）
- `rounded-3xl` >> 用於 >> Hero 元件
- `rounded-3xl` >> 體現 >> 大半徑圓角
- `rounded-2xl` >> 用於 >> 次要內容容器
- `rounded-xl` >> 用於 >> 資訊區塊
- `rounded-xl` >> 用於 >> 群組元素
- `rounded-lg` >> 用於 >> 標準卡片
- `rounded-lg` >> 用於 >> 輸入欄位
- `rounded-md` >> 用於 >> 按鈕
- `rounded-md` >> 用於 >> 邊框容器
- `rounded` >> 等同於 >> `rounded-md`
- `rounded-sm` >> 用於 >> 低調邊框元素
- `rounded-none` >> 用於 >> 工業風格設計
- `rounded-none` >> 對應 >> `0px`
- `rounded-*` >> 屬於 >> Tailwind CSS
- `rounded-*` >> 控制 >> `border-radius`
- Tailwind CSS >> 提供 >> 圓角刻度
- 圓角刻度 >> 確保 >> 視覺一致性
