# reality-indonesia-app
REALITY INDONESIA COMMUNITY 
src/  
├── components/      # Komponen UI (ChatBox, ProjectForm, dll)  
├── pages/           # Halaman (Login, Dashboard, Profile)  
├── services/        # API/Firebase config  
├── assets/          # Gambar/ikon  
└── App.js           # Router utama  
import { getAuth, signInWithEmailAndPassword } from "firebase/auth";  

const handleLogin = (email, password) => {  
  signInWithEmailAndPassword(auth, email, password)  
    .then((userCredential) => {  
      // Redirect ke dashboard  
    })  
    .catch((error) => alert("Login gagal!"));  
};  
