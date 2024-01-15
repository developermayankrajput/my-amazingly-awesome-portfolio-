<script>
    import emailjs from '@emailjs/browser'
    import '@fortawesome/fontawesome-free/css/all.min.css'
    import { faLinkedin } from '@fortawesome/free-brands-svg-icons';
    import { FontAwesomeIcon } from '@fortawesome/svelte-fontawesome';
    function handleSubmit() {
        // Handle form submission logic here
        emailjs
        .sendForm('gmail', 'template_YeJhZkgb', form.current, 'your-token')
        .then(
        () => {
          alert('Message successfully sent!')
          window.location.reload(false)
        },
        () => {
          alert('Failed to send the message, please try again')
        }
      )
    }
</script>
<style>
    li a {
      padding: 7px 0;
      display: block;
      font-size: 15px;
      line-height: 16px;
      color: #4d4d4e;
    }
  </style>
  
<footer id="getintouch" class="py-20 lg:py-20 sm:py-32 bg-[#111111] border border-t border-solid border-cyan-950 flex flex-col gap-4 sm:gap-8 justify-center items-center">
    <p class="px-4 py-2 bg-white text-slate-950 font-medium">
        Contact me &darr;
    </p>
    <form on:submit|preventDefault={handleSubmit} class="max-w-md mx-auto">
        <ul class="list-none p-0">
            <li class="mb-4 flex flex-col lg:flex-row">
                <div class="lg:w-1/2 lg:mr-2">
                    <input
                        placeholder="Name"
                        type="text"
                        name="name"
                        required
                        class="w-full px-4 py-2 bg-gray-300 text-gray-700 border-b-2 border-transparent focus:border-blue-500 transition duration-300 focus:outline-none"
                    />
                </div>
                <div class="lg:w-1/2 sm:w-1">
                    <input
                        placeholder="Email"
                        type="email"
                        name="email"
                        required
                        class="w-full px-4 py-2 bg-gray-300 text-gray-700 border-b-2 border-transparent focus:border-blue-500 transition duration-300 focus:outline-none"
                    />
                </div>
            </li>
            <li class="mb-4">
                <input
                    placeholder="Subject"
                    type="text"
                    name="subject"
                    required
                    class="w-full px-4 py-2 bg-gray-300 text-gray-700 border-b-2 border-transparent focus:border-blue-500 transition duration-300 focus:outline-none"
                />
            </li>
            <li class="mb-6">
                <textarea
                    placeholder="Message"
                    name="message"
                    required
                    class="w-full px-4 py-2 bg-gray-300 text-gray-700 border-b-2 border-transparent focus:border-blue-500 transition duration-300 focus:outline-none"
                ></textarea>
            </li>
            <li>
                <input
                    type="submit"
                    value="SEND"
                    class="float-right px-6 py-3 bg-slate-500 text-white rounded hover:bg-cyan-600 transition duration-300 focus:outline-none"
                />
            </li>
        </ul>
    </form>    
    
    <div class="flex flex-col gap-4 items-center justify-center">
        <p><b class="pr-2">Email</b>mayankrajput40558@gmail.com</p>
        <p class="flex image-center"><b class="pr-2">GitHub</b>
            <img src={"/images/github.png"} alt="github" class="h-5"> 
            <a class="text-cyan-400" target="_blank" href="https://github.com/mayank0rajput"> mayank0rajput</a>
        </p>
        <p class="flex image-center"><b class="pr-2">LinkedIn</b>
            <img src={"/images/linkedin.png"} alt="linkedin" class="h-5"> 
            <a class="text-cyan-400" target="_blank" href="https://www.linkedin.com/in/mayank-rajput-638044227/"> mayank-rajput</a>
        </p>
        <p class="flex image-center"><b class="pr-2">LeetCode</b>
            <img src={"/images/LeetCode.png"} alt="leetcode" class="h-5">
            <a class="text-cyan-400 pd-1" target="_blank" href="https://leetcode.com/mayankrajput40558/"> mayank-rajput</a>
        </p>
        <p>
            <a href="https://www.instagram.com/mayankr253/" target="_blank">Instagram</a>
        </p>
    </div>
</footer>