<div align="center">
  
# Hi there, I'm Ueslei Paim

### Software Engineer | Computer Science Student | Full-Stack Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ueslei-paim-190b09287)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:uesleibros@gmail.com)

</div>

## About me

Greetings! I'm **Ueslei Paim** (aka **UesleiDev**), a passionate software engineer and Computer Science student based in Brazil 🇧🇷.

I specialize in **architecting scalable solutions** and **building robust applications** that solve real-world problems. My expertise spans across **full-stack development**, **system design**, and **automation engineering**. 

With an insatiable curiosity for emerging technologies, I'm constantly exploring new frameworks, design patterns, and best practices to deliver high-quality, maintainable code. I believe in writing **clean code**, following **SOLID principles**, and leveraging **modern development practices**.

### Current Focus
- Pursuing Bachelor's degree in **Computer Science**
- Building innovative solutions for daily challenges
- Deep diving into **software architecture** and **design patterns**
- Exploring **cloud technologies** and **microservices architecture**
- Contributing to open-source projects

### Read me like a code

```py
from __future__ import annotations
from typing import Final, Protocol, runtime_checkable
from dataclasses import dataclass, field
from datetime import datetime
from enum import IntFlag, auto
import threading

@runtime_checkable
class IDeveloper(Protocol):
    """Developer interface."""
    name: str
    location: str
    def code(self) -> None: ...

class Mindset(IntFlag):
    """Developer mindset."""
    CURIOUS = auto()
    PERSISTENT = auto()
    CREATIVE = auto()
    ANALYTICAL = auto()
    
    @classmethod
    def default(cls) -> Mindset:
        return cls.CURIOUS | cls.PERSISTENT | cls.CREATIVE | cls.ANALYTICAL

@dataclass(slots=True)
class UesleiPaim:
    """
    The Developer Himself.
    """
    # Immutable attributes
    name: Final[str] = field(default="Ueslei Paim")
    alias: Final[str] = field(default="UesleiDev")
    location: Final[str] = field(default="Brazil 🇧🇷")
    education: str = field(default="Computer Science Student")
    
    # Private attributes
    _birth_year: int = field(default=2007, init=False, repr=False)
    _started_coding: int = field(default=2017, init=False, repr=False)
    _mindset: Mindset = field(default_factory=Mindset.default, init=False)
    _lock: threading.Lock = field(default_factory=threading.Lock, init=False, repr=False)
    
    @property
    def age(self) -> int:
        """My age."""
        return datetime.now().year - self._birth_year
    
    @property
    def experience(self) -> int:
        """Years of coding experience."""
        return datetime.now().year - self._started_coding
    
    @property
    def currently_learning(self) -> tuple[str, ...]:
        """Current focus areas."""
        return (
            "Algorithms & Data Structures",
            "System Design & Architecture",
            "Low-level Optimization",
            "Cloud Computing",
            "Software Engineering Best Practices"
        )
    
    @property
    def interests(self) -> frozenset[str]:
        """Personal interests (immutable)."""
        return frozenset({
            "Building scalable solutions",
            "Automating repetitive tasks",
            "Open source contribution",
            "Problem solving",
            "Learning new technologies"
        })
    
    @property
    def philosophy(self) -> dict[str, str]:
        """Core beliefs."""
        return {
            "mindset": "Stay curious, stay hungry",
            "code": "Clean code that speaks for itself",
            "learning": "Learn by doing, fail fast, iterate"
        }
    
    def code(self) -> None:
        """What I do best."""
        while True:
            think()
            design()
            implement()
            optimize()
            deploy()
            iterate()
    
    def __repr__(self) -> str:
        return f"<Developer '{self.alias}' | {self.experience} years experience>"
```

## Skills

### Programming Languages

[![Programming Languages-Light](https://skillicons.dev/icons?i=c,javascript,typescript,java,php,lua,python,bash&perline=4&theme=light#gh-light-mode-only)](https://skillicons.dev/icons#gh-light-mode-only)
[![Programming Languages-Dark](https://skillicons.dev/icons?i=c,javascript,typescript,java,php,lua,python,bash&perline=4&theme=dark#gh-dark-mode-only)](https://skillicons.dev/icons#gh-dark-mode-only)

### Markup/Other Languages

[![Extra Languages-Light](https://skillicons.dev/icons?i=html,css,md,latex&perline=4&theme=light#gh-light-mode-only)](https://skillicons.dev/icons#gh-light-mode-only)
[![Extra Languages-Dark](https://skillicons.dev/icons?i=html,css,md,latex&perline=4&theme=dark#gh-dark-mode-only)](https://skillicons.dev/icons#gh-dark-mode-only)

### Databases, Cloud Services and ORMs

[![Databases/Cloud-Light](https://skillicons.dev/icons?i=mongodb,prisma,sqlite,supabase,firebase,googlecloud,mysql,postgresql&perline=4&theme=light#gh-light-mode-only)](https://skillicons.dev/icons#gh-light-mode-only)
[![Databases/Cloud-Dark](https://skillicons.dev/icons?i=mongodb,prisma,sqlite,supabase,firebase,googlecloud,mysql,postgresql&perline=4&theme=dark#gh-dark-mode-only)](https://skillicons.dev/icons#gh-dark-mode-only)

### Tools

#### Collaboration

[![Tools Collaboration-Light](https://skillicons.dev/icons?i=git,github,obsidian,notion&perline=4&theme=light#gh-light-mode-only)](https://skillicons.dev/icons#gh-light-mode-only)
[![Tools Collaboration-Dark](https://skillicons.dev/icons?i=git,github,obsidian,notion&perline=4&theme=dark#gh-dark-mode-only)](https://skillicons.dev/icons#gh-dark-mode-only)

#### In-Production

[![Tools for Development-Light](https://skillicons.dev/icons?i=docker,nginx,graphql,cmake&perline=4&theme=light#gh-light-mode-only)](https://skillicons.dev/icons#gh-light-mode-only)
[![Tools for Development-Dark](https://skillicons.dev/icons?i=docker,nginx,graphql,cmake&perline=4&theme=dark#gh-dark-mode-only)](https://skillicons.dev/icons#gh-dark-mode-only)

#### Libraries/Frameworks

[![Libraries and Frameworks-Light](https://skillicons.dev/icons?i=svelte,jest,react,htmx,vue,vite,nuxtjs,nextjs,webpack,tailwind,solidjs,threejs&perline=4&theme=light#gh-light-mode-only)](https://skillicons.dev/icons#gh-light-mode-only)

[![Libraries and Frameworks-Dark](https://skillicons.dev/icons?i=svelte,jest,react,htmx,vue,vite,nuxtjs,nextjs,webpack,tailwind,solidjs,threejs&perline=4&theme=dark#gh-dark-mode-only)](https://skillicons.dev/icons#gh-dark-mode-only)
