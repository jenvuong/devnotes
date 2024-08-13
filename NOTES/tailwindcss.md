
# TailwindCSS
Everything I have learnt so far in TailwindCSS!

## Using Custom Fonts

#### Step 1. Import the font
Copy the `<link>` tag from the "Embed" section of chosen font.    
Next, add the link to the top of your HTML file.
```
<head>
  <link href="https://fonts.cdnfonts.com/css/telegraf" rel="stylesheet">
</head>
```

#### Step 2. Edit Tailwind configuration
```
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    './index.html',
    './src/**/*.{js,ts,jsx,tsx}'
  ],
  theme: {
    extend: {
      fontFamily: {
        telegraf: ['Telegraf']
      }
    },
  },
  plugins: [],
}
```

#### Step 3. Use the font with Tailwind Classes
```
<h1 className="text-center text-3xl font-bold font-telegraf">Tailwind with custom font!</h1>
```