# ***A Fast File System for UNIX***
*Marshall Kirk McKusick, William N. Joy†, Samuel J. Leffler‡, Robert S. Fabry*
By Computer Systems Research Group, Computer Science Division,Department of Electrical Engineering and Computer Science,University of California, Berkeley

### Motivation:

- The traditional UNIX file system cannot provide sufficient throughput and the locality of reference was not good.

### Contribution(s):
- The paper proposed a reimplementation of the UNIX file system, providing higher throughput without suprising the users with massive change and also discussed enhancements to the programmers' interface.

### Approach:
- The paper first analyzed the traditional UNIX file system and found the reason why the throughput was limited and the locality was poor.
- The new file system used more flexible allocation policies (two possible block sizes), which also made a better locality of reference and could work with various peripheral devices and processers.
- The paper discussed enhancements to the programmers' interface from different aspects: advisory locks on files, namespace extensions across file systems, long file names, and administrative controls over resource usage.

### Strengths:
- The review and analysis about the old file system were very detailed and theoretically convincible.
- The newly proposed system was explained clearly, including the implementation method and the working principles.
- The paper also conducted comprehensive tests to verify the performance of the new system.

### Weaknesses:

- The paper contains so much information and to some extent is not easy to read. When explaining the old and new file system's memory allocation strategy, I think it would be better if there were some figures to help explain the concepts. 
