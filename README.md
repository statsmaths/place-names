# Locating Place Names at Scale

Historical sources are often tagged with metadata about
place such as where the object was created, acquired,
or stored. Rich latent geographical information is often
also mentioned throughout textual documents. A challenge
though is how to extract this spatial information
at scale. For example, when a text mentions Paris, does
the writer mean Paris, Texas, USA or Paris, France? Out
of context, most would assume the reference is to more
populous capital of France, but it could also be the city in
Texas. While close reading would provide an answer, this
becomes a challenge when working with hundreds and
thousands of documents. How might we be able to more
accurately predict the exact location using the broader
context?

Our poster "Locating Place Names at Scale: Using
Natural Language Processing to Identify Geographical
Information in Text" addresses how computational methods
can be used to identify and geolocate place-based
data. We show how Named Entity Recognition (NER), a
natural language processing (NLP) technique, can locate
place names using the document‘s context. We then discuss
how to geolocate those places names using a series
of computational techniques. Specifically, we start by finding
references to specific political divisions (countries,
states, and cities), georeferencing them through the Google
API. Any political divisions that are uniquely determined
become reference points. The reference points are
then used to disambiguate terms with multiple results,
such as Paris, France and Paris, Texas. Disambiguation is
done by appending the political division to the name of the
place in order of specificity. If this fails to uniquely determine
locations, distances to the closest reference points
in the text are used to break ties. This strategy increases
proper place name identification and can be applied automatically
over a large corpus of digitized texts.

Finally, we turn to an example from our collaborative
project on the United States Federal Writers‘ Project
(FWP) entitled Voice of a Nation: Mapping Documentary
Expression in New Deal America. During the New Deal,
thousands of life histories were written to capture the
American experience. While the location of the interviews
provides insight into the geographic expanse of the collection
(Figure 1), the interviewees consistently spoke
about places beyond the location of the physical interview.
We apply NER and NLP to identify the place names
in the interviews. We are then able to identify and map the
many different locations that interviewees mentioned (Figure
2). Across over a thousand interview, what we see is
that many of those interviewed spoke of migration - whether
their own or their kin - generating a more complex
understanding of movement and place during the early
20th century in the United States.
