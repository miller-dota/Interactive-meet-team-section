# Meet Our Teams

A clean, minimal, and interactive team showcase component built with **React**, **TypeScript**, **Vite**, and **Tailwind CSS**.

The component presents a vertical stack of grayscale profile images. Hovering over a team member smoothly expands the selected image while revealing the person's name, role, and short description on either side, creating a lightweight yet engaging interaction.

---

## Preview

See the interaction in action, including hover animations, image scaling, and dynamic content updates.
<p align="center">
 <img src="interaction demo.gif" width="600" />
</p>


### Default State

- Vertical stacked portraits
- Grayscale photography
- Minimal typography
- Center-focused layout

### Hover State

- Active portrait enlarges
- Increased opacity
- Member information animates into view
- Smooth transitions

---

## Features

- Minimal editorial-inspired design
- Vertical image stack
- Hover interactions
- Smooth CSS transitions
- Fully responsive layout
- Grayscale image treatment
- Lightweight implementation
- Easy to customize
- Built with React Hooks
- TypeScript support

---

## Tech Stack

- React
- TypeScript
- Vite
- Tailwind CSS

---

## Project Structure

```text
src/
│
├── app/
│   ├── components/
│   └── App.tsx
│
├── imports/
│
├── styles/
│   ├── globals.css
│   ├── fonts.css
│   ├── index.css
│   ├── tailwind.css
│   └── theme.css
│
└── ...
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/meet-our-teams.git
```

Navigate into the project

```bash
cd meet-our-teams
```

Install dependencies

```bash
pnpm install
```

Start the development server

```bash
pnpm dev
```

---

## Build

Create a production build

```bash
pnpm build
```

Preview production build

```bash
pnpm preview
```

---

## How It Works

Each team member is stored as an object containing:

```ts
{
  name: string
  role: string
  description: string
  photo: string
}
```

The component maps over the array and renders a vertical stack of portraits.

When hovering over a portrait:

- Active index updates using React state
- Selected image expands
- Opacity increases
- Member information updates
- CSS transitions animate the interaction

---

## Customization

### Change Team Members

Simply update the team array.

```ts
const team = [
  {
    name: "Jane Doe",
    role: "Product Designer",
    description: "Crafting delightful user experiences.",
    photo: "/images/jane.jpg"
  }
]
```

---

### Adjust Image Size

Modify the active and inactive dimensions.

```tsx
width: isActive ? 84 : 78
height: isActive ? 96 : 88
```

---

### Transition Speed

```tsx
transition:
"width .25s ease,
height .25s ease,
opacity .25s ease"
```

---

### Grayscale Effect

```css
filter: grayscale(100%);
```

Remove or adjust the filter for full-color portraits.

---

## Responsive Design

The layout is designed to:

- Center content vertically
- Maintain consistent spacing
- Scale smoothly on smaller screens
- Preserve hover interactions on desktop

Mobile interactions can easily be adapted to click/tap events.

---

## Accessibility

- Semantic HTML
- Meaningful image alt text
- Keyboard interaction can be added
- Lightweight DOM structure

---

## Future Improvements

- Keyboard navigation
- Touch-friendly interactions
- Animated text transitions
- Framer Motion support
- Dynamic data fetching
- CMS integration
- Dark mode
- Auto-rotation
- Avatar placeholders
- Scroll-based activation

---

## Dependencies

- React
- TypeScript
- Tailwind CSS
- Vite

---

## License

MIT License

Feel free to use, modify, and distribute this project for personal or commercial work.

---

## Credits

Designed and developed with a focus on minimal interaction design, editorial layouts, and smooth user experience.
