# React + Vite

AI_Resume Builder_Frontend
AI Resume Maker 🚀
A modern, AI-powered resume builder that helps you create professional resumes with ease. Built with React, Vite, and Tailwind CSS.
Show Image
✨ Features

AI-Powered Generation - Leverage AI to generate professional resume content
Multiple Templates - Choose from various professionally designed resume templates
Real-time Preview - See changes instantly as you edit
Export Options - Download your resume as PDF or image
Print Ready - Print-optimized layouts for physical copies
Dark/Light Themes - Multiple theme options powered by DaisyUI
Responsive Design - Works seamlessly on desktop, tablet, and mobile
Form Validation - Smart form handling with React Hook Form
Interactive UI - Smooth animations and particle effects

🛠️ Tech Stack

Framework: React 18.3
Build Tool: Vite 6.0
Styling: Tailwind CSS + DaisyUI
Routing: React Router 7.1
Forms: React Hook Form
HTTP Client: Axios
UI Notifications: React Hot Toast
Icons: React Icons
PDF Generation: React-to-PDF, HTML-to-Image
Effects: React TSParticles

📦 Installation

Clone the repository

bash   git clone <your-repo-url>
   cd resume_frontend

Install dependencies

bash   npm install

Start development server

bash   npm run dev

Open your browser
Navigate to http://localhost:5173

🚀 Available Scripts
CommandDescriptionnpm run devStart development servernpm run buildBuild for productionnpm run previewPreview production buildnpm run lintRun ESLint
📁 Project Structure
resume_frontend/
├── public/              # Static assets
├── src/
│   ├── components/      # React components
│   ├── pages/          # Page components
│   ├── assets/         # Images, fonts, etc.
│   ├── styles/         # Global styles
│   ├── utils/          # Utility functions
│   ├── App.jsx         # Main app component
│   └── main.jsx        # Entry point
├── index.html          # HTML template
├── package.json        # Dependencies
├── tailwind.config.js  # Tailwind configuration
├── vite.config.js      # Vite configuration
└── README.md          # This file
🎨 Themes
The application supports multiple themes via DaisyUI:

Light
Dark
Cupcake
Night (default)

Change theme by updating the data-theme attribute in index.html.
🔧 Configuration
Tailwind Config
Customize your Tailwind setup in tailwind.config.js:
javascriptexport default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {
      // Your custom theme extensions
    },
  },
  plugins: [require("daisyui")],
};
Vite Config
Modify build settings in vite.config.js:
javascriptexport default defineConfig({
  plugins: [react()],
  // Additional configuration
});
📝 Usage Example
javascriptimport { useForm } from 'react-hook-form';
import toast from 'react-hot-toast';

function ResumeForm() {
  const { register, handleSubmit } = useForm();
  
  const onSubmit = (data) => {
    toast.success('Resume updated!');
    // Handle form submission
  };

  return (
    <form onSubmit={handleSubmit(onSubmit)}>
      <input {...register('name')} placeholder="Full Name" />
      <button type="submit">Save</button>
    </form>
  );
}
🌐 Browser Support

Chrome (latest)
Firefox (latest)
Safari (latest)
Edge (latest)

🤝 Contributing
Contributions are welcome! Please follow these steps:

Fork the repository
Create a feature branch (git checkout -b feature/amazing-feature)
Commit your changes (git commit -m 'Add amazing feature')
Push to the branch (git push origin feature/amazing-feature)
Open a Pull Request

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
🐛 Known Issues

PDF generation may have layout issues in some browsers
Print functionality works best in Chrome

🔮 Future Enhancements

 Multi-language support
 Cloud storage integration
 More resume templates
 AI-powered content suggestions
 LinkedIn profile import
 Collaborative editing
 Version history

📞 Support
For support, email support@resumemaker.com or open an issue in the repository.
🙏 Acknowledgments

React
Vite
Tailwind CSS
DaisyUI
All other amazing open-source libraries used in this project
