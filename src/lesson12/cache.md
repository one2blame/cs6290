# Cache

This section conducts a review of the hardware cache. The notes for this lesson
can be found [here](./pdf/Lesson12Notes.pdf)

## Locality

Below is a high-level description from the class describing the concept of
locality.

![locality-principle](./img/locality-principle.png)

The below image from the lectures describes the concepts of
**temporal locality** and **spatial locality**.

![memory-references](./img/memory-references.png)

## Temporal Locality Quiz

The below quiz from the lectures discusses temporal locality with an example
section of code. The `j` and `sum` variables are accessed very often, having
temporal locality in the cache.

![temporal-locality-quiz](./img/temporal-locality-quiz.png)

## Spatial Locality Quiz

We are likely to access all elements of the array in this loop, thus `arr` has
spatial locality.

![spatial-locality-quiz](./img/spatial-locality-quiz.png)

## Cache Quiz

The quiz below describes the concept and purpose of a processor cache.

![cache-quiz](./img/cache-quiz.png)

## Cache Performance

The below excerpt from the class describes the metrics used to measure cache
performance.

![cache-performance](./img/cache-performance.png)

## Hit Time Quiz

This quiz asks some common-sense questions about the timing for a well-designed
cache.

![hit-time-quiz](./img/hit-time-quiz.png)

## Miss Rate Quiz

This quiz asks common-sense questions on the comparison between hit rate and
miss rate.

![miss-rate-quiz](./img/miss-rate-quiz.png)

## Block Size Quiz

The below quiz covers good use of the cache for variables with specific
behaviors.

![block-size-quiz](./img/block-size-quiz.png)

## Block Number Quiz

The below quiz shows us how to calculate the block number.

![block-number-quiz](./img/block-number-quiz.png)

## Cache Tags

The below excerpt from the class describes cache tags.

![cache-tags](./img/cache-tags.png)

## Valid Bit

The below excerpt from the class describes the valid bit.

![valid-bit](./img/valid-bit.png)

## Direct Mapped Cache

The below excerpt from the class describes the direct mapped cache structure.

![direct-mapped-cache](./img/direct-mapped-cache.png)

## Direct Mapped Cache Quiz

The below quiz demonstrates how to find cache conflicts in direct-mapped caches.

![direct-mapped-cache-quiz](./img/direct-mapped-cache-quiz.png)

## Direct Mapped Cache Quiz

Another direct mapped cache quiz showcasing cache conflicts.

![direct-mapped-cache-quiz-2](./img/direct-mapped-cache-quiz-2.png)

## Associative Cache Quiz

The below quiz showcases how we index into an N-way associative cache with an
address.

![associative-cache-quiz](./img/associative-cache-quiz.png)

## Implementing LRU

The below excerpt from the class describes how the LRU policy is implemented for
cache line replacement.

![implementing-lru](./img/implementing-lru.png)

## LRU Quiz

The below quiz demonstrates the LRU cache replacement policy.

![lru-quiz](./img/lru-quiz.png)

## Write Policy

The below excerpt from the lecture provides a good discussion of the differences
between cache writing policies.

![write-policy](./img/write-policy.png)

## Cache Summary

The below excerpt from the course summarizes the data used to handle an example
cache, demonstrating how the cache structure influences the data used to track
the tags, indices, etc.

![cache-summary](./img/cache-summary.png)

## Cache Summary Quiz

Below are the answers to the cache summary quizzes that tie all of these
concepts together.

![cache-summary-quiz](./img/cache-summary-quiz.png)