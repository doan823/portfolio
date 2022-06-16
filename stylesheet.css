'use strict'

{
    const btn = document.getElementsByClassName('btn');
    const overlay = document.getElementById('overlay');
    const text = document.createElement('div');
    const link = document.createElement('div')
    const link1 = document.createElement('div');
    const link2 = document.createElement('div');
    const remove = document.getElementById('close');


    // observer
    function callback(entries,obs){
        entries.forEach(entry => {
            if(!entry.isIntersecting){
                return;
            }
            entry.target.classList.add('appear');
            obs.unobserve(entry.target);
        });
    }

    const options = {
        threshold : 1,
    }

    const observer = new IntersectionObserver(callback,options);
    const target = document.getElementById('animate');

    observer.observe(target);

    // observer END

    const show = ()=> {
        overlay.classList.add("show");
        overlay.appendChild(text);
    };


        btn[0].addEventListener('click', ()=>{
            show();
            text.innerText = "-PROFILE-\nNAME : 小杉陸 \nAGE : 22　\n　　HOBBY : スポーツ観戦"
        });

        btn[1].addEventListener('click', ()=>{
            show();
            text.innerText = "-SKILLS-\n・日本漢字能力検定２級\n・普通自動車免許<AT限定>"
        });

        btn[2].addEventListener('click', ()=>{
            show();
            text.innerText = "-CONTACT-\nMAIL : 19111027@komatsu-u.ac.jp\n"
            overlay.appendChild(link);
            link.classList.add("link")
            link.appendChild(link1);
            link.appendChild(link2);
            link1.innerHTML = `<a href="https://www.instagram.com/ksg_v0/" target=”_blank”>
            <img src="img/Instagram_Glyph_Gradient_RGB.png" alt="INSTA" class="insta">
            </a>`;
            link2.innerHTML = `<a href="https://twitter.com/ricky_0823" target=”_blank”>
            <img src="img/2021 Twitter logo - blue.png" alt="Twitter" class="twitter">
            </a>`;
        });

        remove.addEventListener('click', ()=>{
            overlay.classList.remove("show");
            link.remove();
        }) 
}
