You are a naming assistant. Given a list of file paths and minimal context from a static website, suggest a new filename (basename only, same extension) for each file. Rules:
- Lowercase, kebab-case, no spaces. SEO-friendly and human-readable.
- For HTML: use page purpose (e.g. about-us.html, contact.html). Keep index.html as index.html.
- For CSS/JS: use purpose (e.g. main-styles.css, analytics.js).
- For images: use content (e.g. logo-infygate.webp, hero-banner.webp). Use alt/title when provided.
- Return a JSON object: keys = exact original path strings, values = new basename only (e.g. "main.css"). Preserve extension.
- Do not change path prefix (e.g. css/ stays css/ by returning "name.css" not "css/name.css").

Files and context:
[
  {
    "path": "404.html",
    "context": {
      "title": "",
      "first_heading": "404"
    }
  },
  {
    "path": "Gallery.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "IAPS Photo & Video Gallery"
    }
  },
  {
    "path": "adult-workshop-bengaluru.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Enroll Now for Adult Workshop"
    }
  },
  {
    "path": "css/559e64bf161e61fa0aca6e864c78191d.css",
    "context": {
      "path": "css/559e64bf161e61fa0aca6e864c78191d.css"
    }
  },
  {
    "path": "css/595cb6ccb56826a802ed411cef875f0e.css",
    "context": {
      "path": "css/595cb6ccb56826a802ed411cef875f0e.css"
    }
  },
  {
    "path": "css/84d4a0216f16f715d9b301db3a8da352.css",
    "context": {
      "path": "css/84d4a0216f16f715d9b301db3a8da352.css"
    }
  },
  {
    "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css",
    "context": {
      "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css"
    }
  },
  {
    "path": "css/d09d646f062b67daeff66ff1410b63fc.css",
    "context": {
      "path": "css/d09d646f062b67daeff66ff1410b63fc.css"
    }
  },
  {
    "path": "css/e980cb6b50645ddc9d24377f2fe05d53.css",
    "context": {
      "path": "css/e980cb6b50645ddc9d24377f2fe05d53.css"
    }
  },
  {
    "path": "css/internal-styles.css",
    "context": {
      "path": "css/internal-styles.css"
    }
  },
  {
    "path": "enroll-now-bengaluru.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Enroll Now for Bengaluru"
    }
  },
  {
    "path": "enroll-now-mumbai.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Enroll Now For Mumbai"
    }
  },
  {
    "path": "enroll-now.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Enroll Now for Bengaluru"
    }
  },
  {
    "path": "events.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Enroll Now for Events"
    }
  },
  {
    "path": "franchise.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Upcoming Batches"
    }
  },
  {
    "path": "imgs/0168ef5d8432d48d9b6c4d6ba33e0b7a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/034d0a319d3a9ab4578147bb629ad5db.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/042d59a0f5354fcc31bb047e44139695.webp",
    "context": {
      "refs": [
        {
          "alt": "Public speaking",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0b533918e8f9fb96f7aeb9e66158acd7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0be77d505901964cfaa724d4320c294f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0e9a5e3d4b8717066c1a1d43ddcccbf1.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0ee83fd6a950b1a2e8134f4e5321d89c.webp",
    "context": {
      "refs": [
        {
          "alt": "Increase Self Confidence",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1295faa18daa596aadfffe35335c98b6.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/13dec763e4cdabf5e3e178479f067b85.webp",
    "context": {
      "refs": [
        {
          "alt": "Founder & Director",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/14880f22dfa3600a7218084ca114e9b7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/163070f9fa864c3b52d8c2883d19fb95.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1850fef8ad257e71b4620bc1c13f5888.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1a8dabe8ab87c9ad439eadd3bc7df594.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1c02f16e1bf022a0c01ac4e83df78a7b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1e2e48adcf329b4eacb24fca35c9b8ad.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/20314404edcd3ae2fe4966d4b453426c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/23c0de01bc5e548c06f1e54f7bd7466c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/24b1eef6184011f98365bc8b8c639e19.webp",
    "context": {
      "refs": [
        {
          "alt": "Stage Performance by IAPS Students",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/275771c89df94a7e800faaa0020a59b7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2a2d78cb9950a82d662c242fa46671ad.webp",
    "context": {
      "refs": [
        {
          "alt": "Stage Performance by IAPS Students in Mumbai",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2b148bccdc412d77c7b448ef6493856f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2dffd9e4fe956a9de42b3ac961ec567c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/36cebff0c1e5ff41f08040841f15cfdd.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/39448b39c601d5baadb356d1bbb09267.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3b15f7634e1c3aabcbe26219a5cfd7c6.webp",
    "context": {
      "refs": [
        {
          "alt": "One-to-One Session",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3fb0f380152b74a72b6a79f7c3a825ae.webp",
    "context": {
      "refs": [
        {
          "alt": "Public speaking",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/40a0c012958eec187a2a9fdb1084ea5a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/40fd906befa043c7961983b8b41dd777.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/42207865b71337ea36fb72771865bb2e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/45a09ac7071204af6333b8e84a26dbd6.webp",
    "context": {
      "refs": [
        {
          "alt": "IAPS Speech Competition",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/45abc14d4646dc0195fa679189f85cf1.webp",
    "context": {
      "refs": [
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4ec81d97ed6f40788cd127eee3c4ab9b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/50dcaf58cf4bce7d6311df03393a616c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/50ec03a01a6fb16b7ce219369ba88bc4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/522263309689fe6c395d564e5e8ba0d2.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/529dccd7c3e8162628e4442bb7c8d97a.webp",
    "context": {
      "refs": [
        {
          "alt": "IAPS ONLINE PUBLIC SPEAKING WORKSHOPS FOR KIDS",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/54a57b836901b917a2dc71959c9ac700.webp",
    "context": {
      "refs": [
        {
          "alt": "Increase Self Confidence",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/55377f2fc83236e9f14ebfd16492ec28.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5ac727c5f5673d77bbbeaf31a039ce58.webp",
    "context": {
      "refs": [
        {
          "alt": "IAPS Student Rhea Testimonial Video",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5dfe5639769972ee3acbc20e08055541.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/60af49e4026b577fb38a7b321b4e1d95.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/62f12f0143ec7eb9bce6d9422879a216.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6680f297fbd4b88a6f0e16080bc9e811.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/67d9772917a4b53d3b0bcea4a38b2fd9.webp",
    "context": {
      "refs": [
        {
          "alt": "Public speaking",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/73491a2a8fc861e31055bd962a95290e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/75b6e7c1353a4a214618cbf5af429ad0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7e4f8658ab5fb105ef85341059a419db.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7f2a3b73ad3125b77ac0aca9a8079d8a.webp",
    "context": {
      "refs": [
        {
          "alt": "delivery for kids",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8003ef127b19d183383dc0c59e7e239f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/832385f3a2a47301c0a52dbf696d4b55.webp",
    "context": {
      "refs": [
        {
          "alt": "What parents say about our Public Speaking program",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8551259f1927c7649481b9528897fac6.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/859a31fde5bcbfe7fb0115160ac5eafc.webp",
    "context": {
      "refs": [
        {
          "alt": "Stage performance by IAPS students",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/88b5654a92f73e13eed4275afaa3baf6.webp",
    "context": {
      "refs": [
        {
          "alt": "Public speaking",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8c201504f5aa7974da54cc3e1579f504.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8c99bf0ac6c0f05bfa54746584e0597f.webp",
    "context": {
      "refs": [
        {
          "alt": "IAPS Debate Bootcamp - Apr2019",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/91c8e9c8208f68cdd70c66b7fbd2193c.webp",
    "context": {
      "refs": [
        {
          "alt": "Public Speaking, Tedx",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9aad723625dc335d8ee77517277e207e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9bfd939b4f96531444cfe503fe3b4915.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a015a2283900304fdc302f5563b34b82.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a0ea5bd43447cb681db8b01ba5934c46.webp",
    "context": {
      "refs": [
        {
          "alt": "Sonal S Raja",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a27df3241ac39cf4912b04c149d6c17c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a36f24357be69996b7043195518d66de.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a616416040f65ef8cc3e90e33c0b96d4.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a6373f51537e177603a89ca51ddd674e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b1e22cb501b3b501457a3708145d5d54.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b35ce4ce16a9a6f54ab5b417c4686f91.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b961e7371693d94d7c10625965673179.webp",
    "context": {
      "refs": [
        {
          "alt": "Corporate Trainings",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/bd362bb293bd96bfa81cb74a84c35001.webp",
    "context": {
      "refs": [
        {
          "alt": "IAPS Model United Nations Nov2018",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/bea23410415b975b498780343bc94f1c.webp",
    "context": {
      "refs": [
        {
          "alt": "DEBATE, Public Speaking",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c3fd555a075f48f58a93617a1d3d380d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c98c2ca8f41e04c09727431b8a0a795a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/ccbf9215bd9ac89da130917826c71cca.webp",
    "context": {
      "refs": [
        {
          "alt": "Online Classes",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d0a0321c57262ebe9c39c8835667d92a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d44224c96c1a680b33536ef5dc382e6e.webp",
    "context": {
      "refs": [
        {
          "alt": "IAPS Travel Conclave Jan19",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d4cb384f985c3fd27a01cebc17f65842.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d584a637ca60889d2e02256f77859242.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d8137361cabe1cff55611858e02ad8a2.webp",
    "context": {
      "refs": [
        {
          "alt": "Ashutosh Bhatnagar",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/da4972a732cc95736d22e4be13b7a71e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/dbdffdd57c41c34a373b8d1049091adb.webp",
    "context": {
      "refs": [
        {
          "alt": "Public speaking",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/dc5a3dfaf746c69b907aee9597b8d216.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/dea07116844b5d159422f28246ad5056.webp",
    "context": {
      "refs": [
        {
          "alt": "delivery for kids",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e4aaa432134a8d4ecd544b811e759e64.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e858b1e70d65b14cf40d26cf8239c4e4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/ea890c507dd90a9d0e7baf4f48172a0f.webp",
    "context": {
      "refs": []
    }
  },
  {
    "path": "imgs/eae1e326108491d83a280f02b9ac24ae.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/eafef45efd011657bdce965db93d286a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/ef050c0a0d5086cc92f448fc617d1adc.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f4c364e28149f7209801e273df38dda8.webp",
    "context": {
      "refs": [
        {
          "alt": "Testimonials from parents for IAPS",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f4c9f2057c1d8aa7382c6f62c6e2630b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f4ff1b1c0bf934962cbed0f773ed4fac.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f5227dca15cf5a6e2cace97c0795674b.webp",
    "context": {
      "refs": [
        {
          "alt": "IAPS Travel Conclave",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f804a9375ecb84c55111d0113ac49ab7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/fd306fd2da02bbe6d670970598bc5e61.webp",
    "context": {
      "refs": [
        {
          "alt": "Shruti Jaiswal",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/ff3f4f78846657256343bed64fa4267d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "index.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "About us"
    }
  },
  {
    "path": "js/03b2eaae6007054a68c38e495f894dba.js",
    "context": {
      "path": "js/03b2eaae6007054a68c38e495f894dba.js"
    }
  },
  {
    "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js",
    "context": {
      "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js"
    }
  },
  {
    "path": "js/0c46896987137b0016246f6bc2243099.js",
    "context": {
      "path": "js/0c46896987137b0016246f6bc2243099.js"
    }
  },
  {
    "path": "js/165d7b0ddfa33362140feea997351b77.js",
    "context": {
      "path": "js/165d7b0ddfa33362140feea997351b77.js"
    }
  },
  {
    "path": "js/16df9ef05001a1741857bf99f5a5738f.js",
    "context": {
      "path": "js/16df9ef05001a1741857bf99f5a5738f.js"
    }
  },
  {
    "path": "js/2a85c11e395a8380b5915443e926b569.js",
    "context": {
      "path": "js/2a85c11e395a8380b5915443e926b569.js"
    }
  },
  {
    "path": "js/34be5330971fdbd18985525bd994b0aa.js",
    "context": {
      "path": "js/34be5330971fdbd18985525bd994b0aa.js"
    }
  },
  {
    "path": "js/35c5f9e096d4da33d2a62031daf14248.js",
    "context": {
      "path": "js/35c5f9e096d4da33d2a62031daf14248.js"
    }
  },
  {
    "path": "js/3d70953a848219e749fedc2cdb906675.js",
    "context": {
      "path": "js/3d70953a848219e749fedc2cdb906675.js"
    }
  },
  {
    "path": "js/3e940a33e44b65c1c0af8bb80a893530.js",
    "context": {
      "path": "js/3e940a33e44b65c1c0af8bb80a893530.js"
    }
  },
  {
    "path": "js/544d012df7acf9c3f0920f67c9e322b9.js",
    "context": {
      "path": "js/544d012df7acf9c3f0920f67c9e322b9.js"
    }
  },
  {
    "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js",
    "context": {
      "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js"
    }
  },
  {
    "path": "js/5f5cbb971a3b8261019997ea3a39301c.js",
    "context": {
      "path": "js/5f5cbb971a3b8261019997ea3a39301c.js"
    }
  },
  {
    "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js",
    "context": {
      "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js"
    }
  },
  {
    "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js",
    "context": {
      "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js"
    }
  },
  {
    "path": "js/7260bab328b0ad74815a5efb377bcc67.js",
    "context": {
      "path": "js/7260bab328b0ad74815a5efb377bcc67.js"
    }
  },
  {
    "path": "js/893de96f1b6da546bd7c814964723eca.js",
    "context": {
      "path": "js/893de96f1b6da546bd7c814964723eca.js"
    }
  },
  {
    "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js",
    "context": {
      "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js"
    }
  },
  {
    "path": "js/9455859483e31e4da0e28f10d0742c2a.js",
    "context": {
      "path": "js/9455859483e31e4da0e28f10d0742c2a.js"
    }
  },
  {
    "path": "js/9db10375d298678e53777a2347b87073.js",
    "context": {
      "path": "js/9db10375d298678e53777a2347b87073.js"
    }
  },
  {
    "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js",
    "context": {
      "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js"
    }
  },
  {
    "path": "js/a2261649751fa61b606222c9b2ea3b80.js",
    "context": {
      "path": "js/a2261649751fa61b606222c9b2ea3b80.js"
    }
  },
  {
    "path": "js/b0bade6d42c2702ca85774296cc507c4.js",
    "context": {
      "path": "js/b0bade6d42c2702ca85774296cc507c4.js"
    }
  },
  {
    "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js",
    "context": {
      "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js"
    }
  },
  {
    "path": "js/cecb447a04bbe3e8982190dd6e697120.js",
    "context": {
      "path": "js/cecb447a04bbe3e8982190dd6e697120.js"
    }
  },
  {
    "path": "js/d80b370d82680fc786dcc943a327b9f2.js",
    "context": {
      "path": "js/d80b370d82680fc786dcc943a327b9f2.js"
    }
  },
  {
    "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js",
    "context": {
      "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js"
    }
  },
  {
    "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js",
    "context": {
      "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js"
    }
  },
  {
    "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js",
    "context": {
      "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js"
    }
  },
  {
    "path": "online-workshop.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Enroll Now for WORKSHOPS"
    }
  },
  {
    "path": "privacy-statement.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "PRIVACY STATEMENT"
    }
  },
  {
    "path": "terms-of-service.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "TERMS OF SERVICE"
    }
  },
  {
    "path": "testimonials.html",
    "context": {
      "title": "Indian Academy of Public Speaking | Public Speaking Workshops | Symphysis Training Pvt. Ltd.",
      "first_heading": "Testimonials"
    }
  }
]

Return only a JSON object mapping each path to its new basename (same extension). No other text.