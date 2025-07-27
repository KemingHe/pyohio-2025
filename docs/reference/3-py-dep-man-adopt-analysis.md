# Python Dependency Management Adoption Analysis

> Updated on 2025-07-26 by @KemingHe

Analysis of factors contributing to low formal dependency management adoption in Python repositories, providing context for GitHub adoption statistics.

> [!NOTE]
> Based on [2025-07-27 Adoption Statistics](./2-py-dep-man-adopt-stats.md), the four major dependency managers (pip, Poetry, Conda, UV) collectively cover 2.9% of Python repositories on GitHub. **95+%** lack formal dependency management from major tools.

## Root Causes

### Experimental Development Culture

A 2023 study of **15,817 Python notebooks** from biomedical publications found only **48.31%** declared dependencies, with **41.65%** of failures due to missing dependencies[^1]. This reflects Python's role in experimental and educational contexts where dependency overhead exceeds benefits.

### Dependency Bloat Concerns

Analysis of **1,302 popular Python projects** in 2024 reveals significant inefficiency[^2]:

- **>50%** of dependencies contain unused code
- **87%** of dependency source files go unused  
- **15%** of security vulnerabilities exist in unused code

This drives minimalist approaches, particularly for library authors who "aggressively minimize dependencies" to avoid downstream conflicts[^3].

### Tooling Barriers

Community practitioners report systemic issues: default tooling "makes it almost guaranteed you do the wrong thing," with basic commands potentially breaking system installations[^4]. This creates rational avoidance of formal dependency management.

## Three Distinct Ecosystems

**Educational/Experimental (Majority)**: Tutorial projects, Jupyter notebooks, student assignments using standard library to avoid complexity barriers.

**Standard Library Maximalists**: Leveraging Python's **238 built-in modules** for self-contained solutions without external dependencies.

**Production (Hidden)**: Private repositories, containerized deployments, and enterprise tooling invisible in public GitHub statistics.

## Context-Driven Strategy

Experienced developers apply different approaches[^3]:

- **Libraries**: Extreme minimalism to prevent conflicts
- **Applications**: Liberal dependencies within isolated environments  
- **Scripts**: Zero dependencies for portability

## Strategic Implications

Low adoption reflects rational choices for specific use cases rather than engineering failures. The challenge lies in recognizing transition points from experimental to production-ready dependency management—explaining why technically superior tools like UV struggle despite 10-100x performance advantages.

## References

[^1]: Samuel, S., & Mietchen, D. (2023). Computational reproducibility of Jupyter notebooks from biomedical publications. *arXiv preprint arXiv:2308.07333*. [https://doi.org/10.48550/arXiv.2308.07333](https://doi.org/10.48550/arXiv.2308.07333)

[^2]: Drosos, G. P., Sotiropoulos, T., Spinellis, D., & Mitropoulos, D. (2024). Bloat beneath Python's Scales: A Fine-Grained Inter-Project Dependency Analysis. *Proc. ACM Softw. Eng.*, 1(FSE), Article 114. [https://doi.org/10.1145/3660821](https://doi.org/10.1145/3660821)

[^3]: Nijholt, B. (2025). Confessions of an Asymmetric Hypocrite: On Python Dependencies. *Personal Blog*. [https://www.nijho.lt/post/dependencies/](https://www.nijho.lt/post/dependencies/)

[^4]: Cautaerts, N. (2024). Python dependency management is a dumpster fire. *Personal Blog*. [https://nielscautaerts.xyz/python-dependency-management-is-a-dumpster-fire.html](https://nielscautaerts.xyz/python-dependency-management-is-a-dumpster-fire.html)
