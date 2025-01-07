   
   
   
                    How to install Tailwind Css in your application for Normal Html,js Projects

        1. Initialize Your Project: npm init -y

        2. Install Tailwind CSS Run the following command: npm install -D tailwindcss postcss autoprefixer

        3. Generate Tailwind Configuration: npx tailwindcss init

        4. Set Up Your CSS File Add the following to your styles.css file: 
                                                    
                                                    @tailwind base; 
                                                    @tailwind components; 
                                                    @tailwind utilities;

        5. Configure Tailwind to Process Your CSS Update the tailwind.config.js file to include your HTML files: 

                                module.exports = {
                                    content: ["./*.html"],
                                    theme: {
                                        extend: {},
                                    },
                                    plugins: [],
                                    };

        6. Build the Tailwind CSS File Run the following command to generate your CSS:

                                npx tailwindcss -i style.css -o output.css --watch

        7. Link the Output CSS File In your index.html, link the generated CSS file:
                                
                                <link rel="stylesheet" href="output.css">

        8. Run Tailwindcss : npx tailwindcss init
